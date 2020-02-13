# Civic customization dictionary	
This dictionary includes the names of politicians and journalists, media outlets, cabinet positions, and advocacy/activist groups in the U.S. Also included are general keywords related to U.S. politics. 

We used this dictionary with a (matching program by Chankyung Pak)[https://github.com/pakchank/civic_customization] to compare the lists of pages individuals have liked on Facebook with interests included in individuals' "ad interests" from Facebook. 

As a dictionary, it could be used for a variety of purposes, but given the size (nearly 50,000 items as of Feb. 2020) it would likely be better suited for comparing lists of accounts (e.g., on Twitter)  than for finding evidence of political talk within larger text files. 

## What's included 
This version of the dictionary was last updated March 2019. It includes: 

* Politics (below positions current as of March 2019)
	* The governor for every state 
	* All members of Congress
	* All state legislators 
	* The mayors of the 100 biggest cities in the U.S. 
	* Trump's cabinet (yes, this had to be updated many times)
	* Cabinet positions and major government departments 
* News
	* All journalists who report on politics and current events available in Meltwater's news search database 
	* All news organizations that report on politics and current events (e.g., not entertainment) available in Meltwater's news search database 
* Advocacy and activist organizations on the left and right of the political spectrum 
* Keywords related to news, current events, and politics 

This version was last updated March 2019. 

## Caveats / issues to note 
When making the lists of news and political items, a very broad definition of news and politics was used because we were trying to capture the **possibility** of news and/or politics entering someone's social media newsfeeds. So, groups/pages/organizations/representatives publishing on a platform like Facebook that might **sometimes** post things about news/politics were included in this list. 

But, combined with the (matching program CK Pak made)[https://github.com/pakchank/civic_customization] and the relatively common names of some of these news/politics adjacent publishers, this dictionary + the matching program captures some items that ended up being unrelated to news/politics. 

To deal with this, after running the lists of Facebook pages and ads topics through the matching program, we hand-coded the aggregate lists. We checked each outputted item (Facebook page name or ad topic, after it was run through the matching program) by manually comparing it to the dictionary and searching the output terms on Facebook. If we found a page matching a dictionary term and the outputted terms, we checked the about information for the page and read through the first 20 posts on that page. If none of the posts or self-classified info in the about section were related to news and/or politics, we dropped it from our dataset. 

The best example of this is with the term "film." When specifying outlets and reporters focusing on news/politics/policy reporting, the publisher Film was included in the Meltwater news search database. Because it is such a common word in Facebook pages and ad interests, this one term in the dictionary resulted in many other keywords showing up in the outputted files, so, when hand-coding pages with the term "film"---especially  if they didn't have any posts related to current events or politics---would be removed from the final dataset. 

We've since updated the dictionary to remove terms that either a) caught too many items beyond the specified dictionary item, or b) referenced items unrelated to news/politics. 

## Paper-specific uses & details
This dictionary has been updated over time (see above for details), and so different papers/studies used different versions of the dictionary. 

### Thorson et al., 2019 --- IC&S paper 
For this paper, the March 2017 version of the dictionary was used, with ~30,000 terms in it. 

### Cotter et al. (under review) --- Big Data & Society
For this study, the used March 2019 version of the dictionary was used, with ~50,000 terms in it.  

## References / sources of the data 
BallotPedia. (2017). List of current mayors of the top 100 cities in the United States [Data file]. Available from BallotPedia Web site: [https://ballotpedia.org/List_of_current_mayors_of_the_top_100_cities_in_the_United_States]

The Council of State Governments. (2016). The governors, 2016 [Data file]. Available from The Council of State Governments Web site: [http://knowledgecenter.csg.org/kc/system/files/4.1%202016.xls]

GitHub. (2017). Congress-legislators. Available from GitHub Web site: [https://github.com/unitedstates/congress-legislators]

Meltwater's news search tool 

Open : States. (2017). States [Data file]. Available from Open : States Web site: [https://openstates.org/downloads/]