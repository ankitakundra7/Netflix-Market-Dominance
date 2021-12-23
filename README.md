# Netflix-Market-Dominance
#### - Ankita Kundra, Oluwaseun Ibitoye, Ohyoon Kwon, Ambikha Maharaj, Samuel Oh, Aditya Soni

In this project, we tried to explore if Netflix is beginning to lose its dominance in the streaming services industry through the analysis of user comments on social media. Netflix's streaming services was launched in 2007 and is one of the oldest. This first-mover advantage has helped to ensure its overwhelming dominance in the streaming servies industry for over a decade now. However over the past few years, other streaming platforms such as hulu, hbomax, paramount etc are on the rise. In the first quarter of 2021, Netflix reported the addition of four million new customers which was considerably below the forecasted six million. In this project, we analyze the comments on social media to understand if there is a shift in user sentiments towards Netflix viz-a-viz other streaming services and identify the possible reasons for it.

**Data Preprocessing:**

We scrapped 185,000 comments dating from Jan' 2020 to Oct' 2021 from subreddit r/CordCutters for this purpose. r/CordCutters is a subreddit on Reddit for discussions on live-streaming and on-demand services like Roku, Netflix, Hulu, Amazon, and YouTube TV. We also scrapped comments about Netflix shows on IMDb. 

We began our analysis by cleaning the data. We removed stopwords and punctuations etc. We also replaced different spellings of platform name with a single spelling to make the analysis simpler. For eg.- YouTube TV has been spelt as yttv or youtubetv etc in various comments which was replaced by yttv. Similarly, we replaced different synonyms of attributes we were interested in analyzing with a single word. For eg.- cost was replaced by price. We then removed all the comments in which none of the platforms we are interested in analyzing were mentioned. 

For the purpose of the project, we only analyzed comments which had mention of streaming services: Youtube, Amazon, Hulu, Netflix, HBO Max, Apple, Disney, Sling and Paramount. After Data Cleaning, we were left with 36,500 comments.

**Topic Modeling**

We carried out topic modelling for 36,500 cleaned comments using Latent Dirichlet Alllocation (LDA). LDA represents documents as mixtures of topics that spit out words with certain probabilities. We identified three main topics:
 - Discussions about traditional cable/tv experience (cable, antenna, tv)
 - Discussions about streaming services & their pricing (hbomax, netflix, amazon, price)
 - Discussions about services that offer hardware devices for streaming and their quality (apple tv & roku)

Topic modelling on comments containing Netflix rendered the following topics:
 - Discussions about the company as a whole i.e about the platform, market
 - Discussions about their content, cancelled shows
 - Discussions about netflix in relation to other streaming services (hulu, amazon) and their attributes 


POTENTIAL COMPETITORS - amazon, hbomax
Close cluster - disney, hulu
Potential switching behaviours between clusters 
![image](https://user-images.githubusercontent.com/65372245/147138960-f0431ab0-2f55-46d2-b653-9e4654ae5c72.png)

**Lift Analysis:**


**Sentiment Analysis:**

We find that sentiment scores for all the streaming platforms are positive, ranging between 0.24 and 0.41. Thus, there are no significant insights that can be drawn from the sentiment-score table. Instead of looking at the magnitude of the sentiments, we next looked at the proportion of negative-sentiment and positive-sentiment comments for each platform. We discovered that Netflix had second highest proportion of negative comments among all the platforms. Next, we performed sentiment analysis for specific attributes for each platform. We find that among all the chosen attributes, the proportion of negative comments of Netflix are relatively high for the ‘Family’ and ‘Original’ attributes.
Family
During topic modeling, we found that ‘dark’ was included in the ‘content’ topic. From the table, we can see that there are relatively more negative comments about the family attribute. On the other hand, Disney and Hulu are known to be more family-friendly, which we assumed was why they were not included in the top 3. So this shows how there is a chance of Netflix losing certain subscribers to those family-friendlier platforms.
Original
From the table on the right, we can see that netflix ranks 2nd place for the highest proportion of negative comments about original contents. So we looked into the originals of each of the platforms and found out that netflix actually had the greatest number of original contents. The number of more than all the others’ combined. So we wanted to what aspect of the Netflix’s originals showed areas of improvement and this led to our further investigation about the original content of the platforms.
Lastly, how HBO Max and Amazon are commented about the same attributes in a similar way may underline that they are potential competitors.

![image](https://user-images.githubusercontent.com/65372245/147089976-a93f689f-987c-4914-8ab2-9c06854d4417.png)

**IMDb Comments Analysis:**

The original content is one of the most important features in the TV streaming market. Based on the previous analysis, we decided to compare sentiment scores with IMDb rating of the entire original contents of each platform. The overall trend of this relationship seems to be proportional. We could see that Netfilx’s relatively low scores for both IMDB and sentiment. One issue we thought of is that Netflix might be focusing less on the quality of the contents, compared to the quantity of the contents, which is about 4 times more than the sum of all other streaming services’. 1918 vs 523
![image](https://user-images.githubusercontent.com/65372245/147090022-20ecf13b-d870-49fe-9b73-37e79604e241.png)

any other relevant information regarding netflix dominance, concluding statements
Netflix is still one of the most popular platforms , should not rely on their first mover advantage
Focus on quality over quantity in their original content
The attributes are average compared to the competitors. So improving in any of these will be good (live, connection, etc.)
Biggest competitors: HBOMAX and Amazon
Develop Recommendation System for Platforms → beneficial for people!!!!!
![image](https://user-images.githubusercontent.com/65372245/147090057-37a6fe46-e786-40d2-b1f5-ec3a43ffc52c.png)



