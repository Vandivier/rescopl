<!-- TODO: navbar to get home. maybe https://bootstrap-vue.js.org/docs/components/navbar/ -->

<template>
  <section class="container">
    <div>
      <a class="bookmark"
         :key="arroRows"
         target="_blank"
         v-bind:href="oBookmark.sUrl"
         v-if="oBookmark.sText || oBookmark.sUrl"
         v-for="oBookmark in arroRows">
            {{oBookmark.sText && oBookmark.sText || oBookmark.sUrl}}
      </a>
    </div>
  </section>
</template>

<script>
import axios from 'axios'

const sError = '***ERROR OBTAINING URL***' // technical rule

export default {
    async asyncData () {
        let arroRows = []
        let arrWorkingRow
        let oWorkingRow
        let sWorkingText

        const oResponse = await axios.get('https://raw.githubusercontent.com/Vandivier/site-materials/master/bookmarks.csv')
        const arrsRows = oResponse.data.split(/[\r\n]+/g)

        // split each csv row into an object
        for (let i = arrsRows.length; i--;) {
            arrWorkingRow = arrsRows[i].split(',')
            sWorkingText = arrWorkingRow[1]

            if (sWorkingText !== sError) {
                oWorkingRow = {
                    'sText': arrWorkingRow[1],
                    'sUrl': arrWorkingRow[0]
                }

                arroRows.push(oWorkingRow)
            }
        }

        return { arroRows }
    }
}
</script>

<style>
.container
{
  min-height: 100vh;
  display: flex;
  justify-content: center;
  /* align-items: center; */
  text-align: center;
}
.title
{
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
.subtitle
{
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
.links
{
  padding-top: 15px;
}
.bookmark
{
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
  margin: 7px;
}
.bookmark:hover
{
  color: #fff;
  background-color: #3b8070;
}
</style>
