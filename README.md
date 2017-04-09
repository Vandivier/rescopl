# rescopl - The Research Coordination Platform

### Survey Intro
If I sent you this URL please read this section, otherwise you can skip this. This readme document explains a web application I'm interested in creating, conditional on interest. After review, please send me your response as an interest level [1-5]/5. 1 means you would not use it, 3 maybe, 5 in love. Optionally, send me freeform notes. "I would like it more if X," "my friend would like this," or anything else.

### Main Idea
1. Float and develop an infant idea in an academic-only forum
2. Quickly gauge value and publishing prospects for comparative ideas
3. Recruit co-authors
4. Low on ideas, but ready to work? Become a co-author
5. See what other academics are thinking about as early as possible: Before the working paper

### Candidate Features

**Verified Academics**

Initial validation consists of clicking a link sent to an active .edu email address and a proof document. Proof documents include a link to a teacher's university web page, an image of a degree, or an image of a Ph.D. program acceptance letter. Other users are able to view such proof documents and may raise a possible fraud flag if there is a validity concern.

**Social Features**

Users may log in via Facebook. Users may follow other users and subscribe to notification of their activities. Users may elicit feedback from other users with tagging. Users have profile pages displaying current research topics, background info, and more.

**Reputation**

Users have four reputation metrics: aggregated rep, published citations, idea value, and discussion value. Like Stack Exchange, gain certain abilities by achieving high reputation. For example, access subcommenting and moderator abilities.

**Publicize and Roach Posting**

Eventually the platform may allow users to choose to expose a thread to the public, or even convert the thread into a Stack Exchange or Reddit thread. Roach posts will be hidden to the public, but viewable by other academics, even on public threads.

**Derivative Mapping**

If one idea inspires a related but different idea, you can denote the idea as a derivative idea and specify the differences. This avoids potential conflict by facilitating proper credit even before any citable papers have been yet produced, and it foreshadows citation structure. It also allows the platform to generate an illustrated derivative idea tree or map.

**Discourage Poaching**

Idea contributions are timestamped, so contributing an idea is one way to prove temporal precedence in the origination of an idea. This combats academic poaching, and may be improved when the idea is publicized. Key alternatives to rescopl are inferior means to establish temporal precedence. Derivative mapping also provides a way to avoid temporal ambiguity which can arise when a later idea is published first. Audience control provides an additional layer of protection if desired.

**High-Resolution Voting**

Other sites have a simple up or down vote. This platform uses a 6-option system: Users can vote from 1 to 5 to express their value, or they can vote "undecided/need more info."

**Extensive Idea Evaluation**

Export vote data for complex analysis in the data software of your choice, or utilize built-in quick filters, custom filters, and illustrated report options.

The default value is a linear aggregated vote. Quick filters allow you to weight each vote by user reputation, filter votes by user group, or both. Custom filters allow you to filter or weigh votes by any data available on a user's profile. For example, you might say "show me votes from economists with at least 1 paper actually published, weighted by their citation count." Built-in illustrations are trivial but interesting. For example, visualize the distribution of vote by vote value or show a pie chart of the voters where each slice is a user group.

**Availability Indicator**

Broadcast the approximate number of hours per week you are able and willing to spare for work on a collaborative project.

**Noise Control**

Utilize check boxes to choose which kinds of notifications you want to see. Turn all notifications off, follow certain projects, follow certain users or groups, or follow all activity you are allowed to see. See notifications only in the app or in your inbox. Add a second inbox so it doesn't have to use your academic address.

**Audience Control**

Like Facebook, control who is allowed to view or be notified of your contributed ideas. Select particular users or leverage user groups. Choose whether your idea is public or private. Everything is private by default. Audience settings can be edited over time.

**3-View Idea Page**

Each idea you submit will have a discussion page with three views. The default view is a summary view which displays the users who have voted, the direction of their vote, and their aggregated reputation. Note that this is different from Reddit or other social sites. Other sites present your aggregate score, but they do not detail the underlying users and votes. This is important in case you want to drill down and elicit feedback directly.

The second page is a discussion page which looks like Stack Exchange. Individuals optionally post comments which can be up or downvoted. Top comments rise to the top. Subcomments may be added to the original post or any comment. Subcomments may not be downvoted and are not reordered, to facilitate in-depth discussion without fear of downvoting.

**Idea Tags and Fields**

Other websites use tags and categories, but the platform will use journal-recognized field codes where applicable. Relevant jargon or arbitrary text may be linked to an idea with a tag. Research other ideas based on tags, fields, date range, and other filters.

**Idea Lifecycle**

Contribute an infant idea, develop it in conversation on the platform, associate the idea with a working paper, associate grants awarded, and, finally, associate the resulting paper. In theory, there should be one paper per idea. A second paper should involve a new idea, even if the new idea is to replicate an old idea. As data grows, eventually the platform may be able to estimate lifecycle outcomes based on the idea tags, fields, or other properties.

**Featured Ideas**

Like Stack Exchange, offer some of your reputation in exchange for expedited review and featured status. Users who give you the feedback you are looking for within your specified time frame receive a fraction of the reputation offered. If no feedback is received, no reputation is lost.

### Parts Unsure
1. The name
2. WordPress or standalone NoSQL + Node back end
3. React, MarkoJS, or other front end framework
4. Implement a scrum feature set including projects and tasks
5. Timeline. This depends on interest and whether or not funding is obtained
