# Moreyball
Long term goals:

- [ ] Create a comprehensive database
- [ ] Project win spreads
- [ ] Create a metric that measures 'value' and/or plus-minus
- [ ] Project value

Short term goals:

- [ ] Download data from BBR and NBA.com (or other sites)
- [ ] Team scoring efficiency vs wins/expected wins
- [ ] Team scoring efficiency vs net rating/overall rating

Medium(?) term goals (just spitballing here):

- [ ] Individual physical measurements vs team defensive performance
- [ ] Team physical measurements/variance vs team defensive performance
- [ ] Individual scoring efficiency vs team offensive/overall performance
- [ ] Team scoring efficiency vs team offensive/overall performance
- [ ] Individual scoring efficiency vs individual usage rate

Analytics 'conventional wisdom' that I'd like to test at some point:

- [ ] As predictive metrics, RPM > WS, VORP > BPM, PER
- [ ] There are no publicly available statistics that adequately measure individual defense (Daryl Morey quote, this will be quite difficult to test because judging defense is extremely dependent on the 'eye test,' which is deeply flawed in its own way)
- [ ] For rookies coming from the NCAA (college ball), NCAA FT% or a blend of NCAA FT%/3P% are better indicators of NBA 3P% than NCAA 3P%
- [ ] Any defensive metrics that rely on box score stats will necessarily overvalue players who can accumulate rebounds, steals, or blocks; these are the only defense-related box score stats (besides simple plus-minus) but hardly capture a player's entire defensive ability

# The Eye Test
At various points I have described the 'eye test' or conclusions that I've reached through watching the NBA. Ideally, any meaningful conclusions we can reach through statistical analysis should be verified by a corresponding, independently derived 'eye test' conclusion. Of course, both statistics and the 'eye test' are flawed, so this is hardly perfect, but there are some broad 'eye test' conclusions that I'm confident enough in to use as measuring sticks for our analysis:

- Russell Westbrook's counting statistics are vastly overinflated compared to his impact on the court, thus, any model that values him over, say, James Harden or Stephen Curry, places far too much reliance on counting stats. Similarly, any model that counts Westbrook or John Wall as the best passers in the league overvalues assists. As Daryl Morey once said, 'there is no (box score) statistic that cannot be accummulated selfishly.' Especially for the big three of points, rebounds, and assists, efficiency is far more important for success than volume.  
- Stephen Curry's off-ball impact on his team's offense is otherworldly. His 'gravity' is era-defining. Any offensive plus-minus metrics should rate him very highly.
- Switching on defense is the name of the game. Switch-heavy defenses need versatile defenders. What does this mean in terms of numbers? The best defenses have the least variation in height (broadly speaking). The ideal is to have five players between 6'6"-6'10", or 198-208 cm.

# Miscellaneous Stuff
I don't imagine that our project will be as ambitious as CARMELO, but take a look at FiveThirtyEight's explanation of their methodology, because I think a lot of useful insights can be gained. I posted the interactive in the initial email, so feel free to play around with that to learn exactly what CARMELO is trying to do.
- 2015-16 (launch year): https://fivethirtyeight.com/features/how-were-predicting-nba-player-career/
- 2016-17: https://fivethirtyeight.com/features/whats-new-in-our-nba-projections-for-2016-17/
- 2017-18: https://fivethirtyeight.com/features/whats-new-in-our-nba-player-projections-for-2017-18/
- 2018-19: https://fivethirtyeight.com/features/our-nba-player-projections-are-ready-for-2018-19/

So from reading these pieces, I've come to a few early conclusions: firstly, BPM (Box Plus Minus) is trash compared to RPM (Real Plus Minus, also called RAPM). Second, BBR (basketball-reference.com) is not the best place to find physical measurements and players' positions. For those purposes, NBA.com and ESPN Fantasy Basketball, respectively, are superior. Third, projecting the performance/value of rookies is difficult, given the relative sparsity of data available on college and EuroLeague basketball, which are the two main sources of rookies. We will not be getting involved in that for the forseeable future.


RealGM, the biggest online basketball forum, has a Statistical Analysis board (among others). Reddit has r/nba and r/nbadiscussion, with the former being the huge meme-filled subreddit and the latter being a tiny but more serious sub. Often when I'm procrastinating I find myself browsing through these forums, and I'll warn you that the signal-noise ratio is awful. Just god-awful. If you have to look at one look at the RealGM board, but even so, most of the posters and discussion are trash-tier. There are some nuggets of wisdom, but I don't expect you to put in the time necessary to find them. 
- https://forums.realgm.com/boards/viewforum.php?f=344
- https://old.reddit.com/r/nba/
- https://old.reddit.com/r/nbadiscussion/


In general, when thinking about effective team building and judging NBA players, the notions of value and surplus value (or, as I call it, 'generating value') are of the utmost importance to me. This is the main goal of analysing statistics for me, and everything we do should have an eventual connection to value. I've been highlighting CARMELO because it also has this goal in mind, measuring value both in WAR (Wins Above Replacement) and market value. The following articles capture some, though hardly all, of my thoughts about value generation:
- https://fivethirtyeight.com/features/carmelo-anthonys-contract-could-doom-the-knicks-to-mediocrity/
- https://fivethirtyeight.com/features/russell-westbrook-is-really-worth-344-million-and-other-tales-of-the-nbas-new-salary-cap/
- http://www.espn.com/pdf/2016/0406/nba_hinkie_redact.pdf


The following is another small project that I found a while ago and forgot to include in the email. This one measures the success of draft picks, and though the methodology is simplistic compared to the others, it represents a more attainable goal. The first link describes the project, the second is the data used, and the third is data from an unrelated third party about the performance of draft picks.
 - https://old.reddit.com/r/nba/comments/8v1awu/oc_a_new_statistic_evaluating_every_draft_pick/
 - https://docs.google.com/spreadsheets/d/1H3lMr8UO2YIwnKKXrpySzWyReFMzly_TLOQVjLNTQzE/edit#gid=2021074514
 - https://github.com/jbmoskow/The-Process-Revisted

# Initial Email
Sorry for not updating you earlier, but I've been looking into basketball analytics for most of the summer, and though admittedly I haven't gotten a start with the coding and haven't studied enough linear algebra/statistics, I've found quite a few resources from which we can draw data and ideas for the direction of the project.


So these first few articles I sent you are not directly related to analytics, but they provide context for where this project fits in the bigger picture.

- http://grantland.com/the-triangle/future-of-basketball-james-harden-daryl-morey-houston-rockets/
- http://www.slate.com/articles/arts/books/2016/12/how_daryl_morey_used_behavioral_economics_to_revolutionize_the_art_of_nba.html
- http://www.espn.com/pdf/2016/0406/nba_hinkie_redact.pdf

Of course, coding/statistics experience is still the main goal, and perhaps for you it is the only goal (nothing wrong with that), but in my mind analytics is one step towards a larger aim: developing a more effective system of reasoning about sports by using Bayesian probability as a foundation. It is quite clear to me that Daryl Morey and Sam Hinkie are also firmly committed to this idea, as can be extrapolated from the above articles. They have been rather successful in the NBA by using this approach, so, broadly speaking, I take my cues from them.


Now, moving onto the meat of the project, I've found quite a few sites that compile NBA statistics. These two are by far the most useful:

BBR is my first and (often) last stop for stats. It compiles traditional counting, or 'box score' stats, as well as the massive number of advanced statistics that are calculated from box score stats. It has the best site design and search tools of all the sites I've found.
- https://www.basketball-reference.com/play-index/

Disclaimer: NBA.com has a much shittier design than BBR. However, it is one of the most useful because they compile certain (very useful) stats that no one else can. The format is hardly ideal and most of the data will be irrelevant to us, but sifting through that is a job for later.
- http://stats.nba.com/

Other potential sources of data (warning most of the websites are poorly designed):

We're not using SQL, so we can ignore this one for now, but in case we do this will be immensely useful.
- https://drive.google.com/drive/folders/19WhE2lveFtVrQimmLPGWpqfooejMTwNo

Play-by-play stats, shot charts, and other things that could be useful but aren't immediately relevant.
- http://www.pbpstats.com/

Pretty gross websites. Ideally we would avoid these but...just in case we need more.
- https://nbamath.com/nba-math-statistics/
- http://hoopdata.com/advancedstats.aspx

There are a lot of strange acronyms and terms thrown around, so these are useful glossaries:
- https://www.basketball-reference.com/about/
- https://www.nbastuffer.com/analytics-101/


So, what will our project be about? I admit that I don't quite know yet, but here are some existing projects that can guide us:

This person is good. Real good. Now, he/she has significantly more experience with data science and machine learning than we do, but if you do want to delve into machine learning, we can attempt some things resembling this person's work. Of course, to do so would involve studying statistics and machine learning concepts more than actual coding.
- https://old.reddit.com/user/dribbleanalytics/posts
- https://github.com/dribbleanalytics

The other major existing project I want to highlight is FiveThirtyEight's CARMELO. The first link is an interactive, the second (partially) explains the methodology, and the third contains the source data. Now, from my existing knowledge of the NBA, the results CARMELO produces are...suspect. However, I like their methodology, in particular their use of 'similarity scores,' and I think that their goal, projecting 'value above replacement' (the concept, not VORP the advanced stat), is one of the things that makes the most sense for a long term project (with the other being projecting win spreads).
- https://projects.fivethirtyeight.com/carmelo/
- https://fivethirtyeight.com/features/our-nba-player-projections-are-ready-for-2018-19/
- https://github.com/fivethirtyeight/data/tree/master/nba-carmelo

