# Moreyball
Long term goals:
Create a comprehensive database
Project win spreads
Create a stat that measures 'value'
Project value

Short term goals:
Download data from BBR and NBA.com (or other sites)

Medium(?) term goals (just spitballing here):
Individual physical measurements vs team defensive performance
Team physical measurements/variance vs team defensive performance
Individual scoring efficiency vs team offensive/overall performance
Team scoring efficiency vs team offensive/overall performance

# Initial email
Sorry for not updating you earlier, but I've been looking into basketball analytics for most of the summer, and though admittedly I haven't gotten a start with the coding and haven't studied enough linear algebra/statistics, I've found quite a few resources from which we can draw data and ideas for the direction of the project.


So these first few articles I sent you are not directly related to analytics, but they provide context for where this project fits in the bigger picture.

http://grantland.com/the-triangle/future-of-basketball-james-harden-daryl-morey-houston-rockets/

http://www.slate.com/articles/arts/books/2016/12/how_daryl_morey_used_behavioral_economics_to_revolutionize_the_art_of_nba.html

http://www.espn.com/pdf/2016/0406/nba_hinkie_redact.pdf

Of course, coding/statistics experience is still the main goal, and perhaps for you it is the only goal (nothing wrong with that), but in my mind analytics is one step towards a larger aim: developing a more effective system of reasoning about sports by using Bayesian probability as a foundation. It is quite clear to me that Daryl Morey and Sam Hinkie are also firmly committed to this idea, as can be extrapolated from the above articles. They have been rather successful in the NBA by using this approach, so, broadly speaking, I take my cues from them.


Now, moving onto the meat of the project, I've found quite a few sites that compile NBA statistics. These two are by far the most useful:

https://www.basketball-reference.com/play-index/
BBR is my first and (often) last stop for stats. It compiles traditional counting, or 'box score' stats, as well as the massive number of advanced statistics that are calculated from box score stats. It has the best site design and search tools of all the sites I've found.

http://stats.nba.com/
Disclaimer: NBA.com has a much shittier design than BBR. However, it is one of the most useful because they compile certain (very useful) stats that no one else can. The format is hardly ideal and most of the data will be irrelevant to us, but sifting through that is a job for later.


Other potential sources of data (warning most of the websites are poorly designed):

https://drive.google.com/drive/folders/19WhE2lveFtVrQimmLPGWpqfooejMTwNo
We're not using SQL, so we can ignore this one for now, but in case we do this will be immensely useful.

http://www.pbpstats.com/
Play-by-play stats, shot charts, and other things that could be useful but aren't immediately relevant.

https://nbamath.com/nba-math-statistics/
http://hoopdata.com/advancedstats.aspx
Pretty gross websites. Ideally we would avoid these but...just in case we need more.

There are a lot of strange acronyms and terms thrown around, so these are useful glossaries:
https://www.basketball-reference.com/about/
https://www.nbastuffer.com/analytics-101/


So, what will our project be about? I admit that I don't quite know yet, but here are some existing projects that can guide us:

https://old.reddit.com/user/dribbleanalytics/posts
https://github.com/dribbleanalytics
This person is good. Real good. Now, he/she has significantly more experience with data science and machine learning than we do, but if you do want to delve into machine learning, we can attempt some things resembling this person's work. Of course, to do so would involve studying statistics and machine learning concepts more than actual coding.

https://projects.fivethirtyeight.com/carmelo/
https://fivethirtyeight.com/features/our-nba-player-projections-are-ready-for-2018-19/
https://github.com/fivethirtyeight/data/tree/master/nba-carmelo
The other major existing project I want to highlight is FiveThirtyEight's CARMELO. The first link is an interactive, the second (partially) explains the methodology, and the third contains the source data. Now, from my existing knowledge of the NBA, the results CARMELO produces are...suspect. However, I like their methodology, in particular their use of 'similarity scores,' and I think that their goal, projecting 'value above replacement' (the concept, not VORP the advanced stat), is one of the things that makes the most sense for a long term project (with the other being projecting win spreads).
