# Netflix-Market-Dominance
#### - Ankita Kundra, Oluwaseun Ibitoye, Ohyoon Kwon, Ambikha Maharaj, Samuel Oh, Aditya Soni

In this project, we tried to explore if Netflix is beginning to lose its dominance in the streaming services industry through the analysis of user comments on social media. Netflix's streaming services was launched in 2007 and is one of the oldest. This first-mover advantage has helped to ensure its overwhelming dominance in the streaming servies industry for over a decade now. However over the past few years, other streaming platforms such as hulu, hbomax, paramount etc are on the rise. In the first quarter of 2021, Netflix reported the addition of four million new customers which was considerably below the forecasted six million. In this project, we analyze the comments on social media to understand if there is a shift in user sentiments towards Netflix viz-a-viz other streaming services and identify the possible reasons for it.

**Data Preprocessing:**

We scrapped 185,000 comments dating from Jan' 2020 to Oct' 2021 from subreddit r/CordCutters for this purpose. r/CordCutters is a subreddit on Reddit for discussions on live-streaming and on-demand services like Roku, Netflix, Hulu, Amazon, and YouTube TV. We also scrapped comments about Netflix shows on IMDb. 

We began our analysis by cleaning the data. We removed stopwords and punctuations etc. We also replaced different spellings of platform name with a single spelling to make the analysis simpler. For eg.- YouTube TV has been spelt as yttv or youtubetv etc in various comments which was replaced by yttv. Similarly, we replaced different synonyms of attributes we were interested in analyzing with a single word. For eg.- cost was replaced by price. We then removed all the comments in which none of the platforms we are interested in analyzing were mentioned. 

For the purpose of the project, we only analyzed comments which had mention of streaming services: Youtube, Amazon, Hulu, Netflix, HBO Max, Apple, Disney, Sling and Paramount. After Data Cleaning, we were left with 36,500 comments.

**Topic Modeling**

We carried out topic modelling for 36,500 cleaned comments using Latent Dirichlet Allocation (LDA). LDA represents documents as mixtures of topics that spit out words with certain probabilities. We identified three main topics:
 - Discussions about traditional cable/tv experience (cable, antenna, tv)
 - Discussions about streaming services & their pricing (hbomax, netflix, amazon, price)
 - Discussions about services that offer hardware devices for streaming and their quality (apple tv & roku)

Topic modelling on comments containing Netflix rendered the following topics:
 - Discussions about the company as a whole i.e about the platform, market
 - Discussions about their content, cancelled shows
 - Discussions about netflix in relation to other streaming services (hulu, amazon) and their attributes 


**MDS Plot:**

MDS arranges the points on the plot so that the distances among each pair of points correlates as best as possible to the dissimilarity between those two samples.
MDS ploy shows that amazon and HBO Max are potential competitors of Netflix. Another close cluster is that of Disney and Hulu. There can be switching behaviours between clusters.

**Lift Analysis:**

Lift analysis shows that Netflix has high association with the attribute 'unsubscribe' and 'original'. This may indicate that people are talking about unsubscribe when they are talking about Netflix more often. 


**Sentiment Analysis:**

We find that sentiment scores for all the streaming platforms are positive, ranging between 0.24 and 0.41. Thus, there are no significant insights that can be drawn from the sentiment-score table. Instead of looking at the magnitude of the sentiments, we next looked at the proportion of negative-sentiment and positive-sentiment comments for each platform. We discovered that Netflix had second highest proportion of negative comments among all the platforms. Next, we performed sentiment analysis for specific attributes for each platform. We find that among all the chosen attributes, the proportion of negative comments of Netflix are relatively high for the ‘Family’ and ‘Original’ attributes.

Family:
During topic modeling, we found that ‘dark’ was included in the ‘content’ topic for Netflix. During sentimental analysis, it is also observed that there are relatively more negative comments about the family attribute for Netflix. On the other hand, Disney and Hulu are known to be more family-friendly. Hence, it might be the case that Netflix is losing certain subscribers to those family-friendlier platforms.

Original:
Netflix ranks at second place for the highest proportion of negative comments about original contents. We looked into the originals of each of the platforms and found that netflix has more number of original-content shows than all the other platforms combined. This piqued our interest in knowing the possible areas of improvement in Netflix’s original content which would be investigated in the next section.
Lastly, high association between HBO Max and Amazon with 'originals' attribute might indicate that they are potential competitors of Netflix.

**IMDb Comments Analysis:**

The original content is one of the most important features in the streaming services industry. Based on the previous analysis, we decided to compare sentiment scores with IMDb rating of the entire original contents of each platform. The overall trend of this relationship seems to be proportional. Netflix has relatively low scores for both IMDB and sentiment scores. One possible reason could be Netflix's focus on quantity over quality.


**Conclusions and Recommendations:**

It can be concluded from the analysis that Netflix is still the most dominant player in the streaming-services industry but competitors are fast catching up. It cannot continue to rely on the first mover advantage. Netflix's biggest competitors according to our analysis are: HBOMAX and Amazon. Netflix should focus on quality over quantity in their original content. Many attributes have an average sentiment score for Netflix compared to its competitors. So improving upon any of these attributes (originality, live, connection, etc.) might help to improve the sentiments about Netflix.



