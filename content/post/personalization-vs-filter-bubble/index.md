---
title: "Personalization versus 'Filter Bubble': The Influence of Personalization on the Quality of Search Queries"
subtitle:

# Summary for listings and search engines
summary: With the accelerating speed of data generation, it becomes increasingly important to develop and improve techniques which help us find the most relevant information for any given question. Personalization as a solution  is satisfactory for many use cases, such as on-site search in e-commerce or many queries on general purpose search engines. For certain queries, such as those on controversial political topics, however, result diversity is important to diminish the negative effects of personalization on civic discourse and democracy.

# Link this post with a project
projects: []

# Date published
date: "2018-10-17"

# Date updated
# lastmod: 

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

authors:
- admin

---

_This essay was originally written in May 2017 and submitted as part of my application for TU Munich's [Data Engineering and Analytics Master program](https://www.in.tum.de/en/for-prospective-students/masters-programs/data-engineering-and-analytics-msc/). For better or worse, I have not been admitted, but I wanted to share an edited version of the essay so that the effort has not been in vain, in particular because I think that this issue is still extremely relevant and not nearly enough effort has been undertaken to tackle it._

## Introduction
With the accelerating speed of data generation, it becomes increasingly important to develop and improve techniques which help us find the most relevant information for any given question. Personalization describes a set of filtering and sorting techniques aimed at achieving this goal by sorting information by its relevance for a specific user, often accompanied by removing results that are deemed irrelevant. To infer the relevance, personalization uses information about the user such as profile-based data (e.g. gender and location) and behaviour-based data (e.g. previously clicked search results) ([Dou et al., 2007](https://doi.org/10.1145/1242572.1242651)). Critics however are concerned about the effect of personalization on civic discourse and about the phenomenon of “filter bubbles”, where users would only receive information supporting their personal beliefs and no content which challenges these beliefs and offers a broader perspective ([The Guardian, 2017](https://www.theguardian.com/media/2017/jan/08/eli-pariser-activist-whose-filter-bubble-warnings-presaged-trump-and-brexit)). In particular, Donald Trump winning the 2016 Presidential election raised such concerns with [WIRED (2016)](https://www.wired.com/2016/11/filter-bubble-destroying-democracy/) arguing that Trump’s win was supported by filter bubbles.

An important question is therefore how personalization influences the quality of search results and if it serves as a suitable improvement. Over the course of this essay I will demonstrate the necessity of personalization of search results to cope with the increasing amounts of data and that it improves the quality of search results. Nonetheless, I will also argue that the definition of quality used in academic research is not sufficient for controversial topics and must be extended to promote result diversity in order for users to take informed decisions. A discussion of privacy issues related to personalization is beyond the scope of this essay.

## Personalization helps cope with information overflow
As mentioned above, the speed of data generation is constantly increasing, while the information processing capabilities of a human are capped. Once information overload occurs, human performance declines rapidly, creating the need for techniques to manage information and prevent information overload ([Bozdag, 2013](https://doi.org/10.1007/s10676-013-9321-6)). By focusing on individual relevance of information, search result personalization has suitable theoretical properties to be such a technology. Empirical research supports this theoretical intuition: [Dou et al. (2007)](https://doi.org/10.1145/1242572.1242651) showed that click-based personalization is able to improve search. The study used click-through data from MSN and compared different personalization strategies and non-personalized search using rank-scoring and the average rank as metrics. Their implementation of profile-based personalization did not improve search results, yet another study by Sieg et al. (2007) demonstrated that re-ranking search results based on user interests is able to increase both precision and recall when comparing the top-n results of personalized and non-personalized search queries. Moreover, [Goldman (2008)](https://doi.org/10.1007/978-3-540-75829-7_8) argues that personalization diminishes the effects of search engine bias created by ranking of results based on popularity.

## Limited exposure to different opinions harms civic discourse
Critics of personalization however have attributed it with the creation of so-called “filter bubbles”, where personalization engines isolate internet users in their “unique universe of information” ([Pariser, 2012](https://dl.acm.org/citation.cfm?id=2361740)). This is caused by presenting only information that the system identifies as relevant for the user, which leads to filtering out information that disagrees with their personal viewpoints. While there is little academic research on the extent of the existence of filter bubbles in search engines, negative effects of exposure to a limited set of opinions on civic discourse have been shown: [Zuiderveen Borgesius et al. (2016)](https://doi.org/10.14763/2016.1.401) found that the people with regular exposure to biased content are less able to understand opposing views or give reasons for their own choices while also developing more polarizing views.

The extent to which current search engines promote result diversity is unclear. As [Slate (2011)](http://www.slate.com/articles/news_and_politics/the_big_idea/2011/06/bubble_trouble.html) reports, Google claims to promote diverse results, yet it is intransparent how personalization is used to filter and rank search results. According to [Hannak et al. (2013)](https://doi.org/10.1145/2488388.2488435), on average 11.7% of search queries on Google are personalized, but they could only detect logged-in users and the IP address of a user as a source for personalization. This intransparency was also publicly criticized by the Council of Europe [in 2012](https://search.coe.int/cm/Pages/result_details.aspx?ObjectID=09000016805caa87
) as a potential threat to “\[h]uman rights and fundamental freedoms”. For academic research on personalization in recommendation engines, [Zhang et al. (2012)](https://doi.org/10.1145/2124295.2124300) argue that commonly used measurements are focused on the accuracy of the results, such as the click-through based scoring in [Dou et al. (2007)](https://doi.org/10.1145/1242572.1242651). By design, these are therefore self-limiting on a subset of possibly relevant recommendations  and do not aim at exposing the user to the maximum available number of relevant content.

For controversial topics such as political issues, where users should make informed decisions, it is important for civic discourse that the users are exposed to a broad range of items, some of them they may disagree with. To illustrate the difference to other searches, compare the following scenarios: If a user wants to book a hotel in Barcelona, user intent is satisfied if the results are pre-filtered to the most relevant hotels and booking sites that fit the user’s needs and profile. If a user seeks information about an issue such as the Affordable Care Act, reliable sources should be displayed that take different angles on the issue, some of them disagreeing with the user’s personal beliefs but helping in understanding the opposing site. [Zhang et al. (2012)](https://doi.org/10.1145/2124295.2124300) introduced measures for diversity and serendipity to evaluate the performance of a music recommendation engine and demonstrated an increase in user satisfaction. For an understanding of the influence of these measures on result diversity in search engines further research is required.
 
## Conclusion
In conclusion, personalization is improving search queries with regard to the relevance of the displayed results. This is satisfactory for many use cases, such as on-site search in e-commerce or many queries on general purpose search engines. For certain queries, such as those on controversial political topics, however, result diversity is important to diminish the negative effects of personalization on civic discourse and democracy. Search engines can promote this by including measures for diversity and serendipity in their evaluation metrics. Further research needs to be done on the effects and efficiency of this model of diversity promotion, the extent to which personalization is happening at the moment as well as the methodologies that are in use.
