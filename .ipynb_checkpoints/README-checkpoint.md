## Shaping Presidential Policies Using Rappler Articles
![Header](Header.png)

## Abstract

This comprehensive study employs Latent Semantic Analysis (LSA) to examine dominant themes in news articles from Rappler concerning President Bongbong Marcos' first year in office. Aimed at enhancing policy-making, strategic communications, and public engagement, the research focuses on analyzing media narratives to provide insights into public discourse and political events. The study identifies three primary clusters: "Political Alliances and Dynasties," "Media and Disinformation," and "International Relations and Economic Policies." These insights offer a nuanced understanding of media portrayal and public perception of political events and policies, aiding in the formulation of strategies for policy analysis, public relations, and speech building.

## Skills and Tools Employed
- **Data Collection from Online News Sources**
- **Advanced Data Cleaning Techniques**
- **Customized Database Management**
- **Demographic and Sentiment Analysis**
- **Trend Analysis During Specific Political Periods**
- **Cultural Insight Integration**
- **Web Scraping**:
  - `bs4` (BeautifulSoup): For pulling data out of HTML and XML files
- **Text Processing and Analysis**:
  - `sklearn.feature_extraction.text` (TfidfVectorizer): For creating Bag-of-Words subjected to TF-IDF
- **Clustering**:
  - `sklearn.cluster` (KMeans): For performing K-Means clustering
  - `yellowbrick.cluster` (KElbowVisualizer): For finding the optimal number of K-Means clusters

## Data Sources and Description

### Dataset Used
- The main dataset is obtained from Rappler using the search prompt "Marcos year 2022."
- The dataset contains 100 articles, each with the following variables:
  - Title
  - Link

### Data Assumptions and Limitations
- **Representativeness**: The dataset is presumed to represent the overall media coverage regarding President Marcos's administration.
- **Time-Bound Analysis**: The study focuses on articles from a specific time period.
- **Scope of Data**: The dataset is confined to a single news source, Rappler.
- **Stability of Online Content**: Assumes that the content of the articles has remained unchanged since publication.
- **Potential Bias in Source Selection**: The exclusive use of Rappler could introduce bias in the analysis.

## Methodology

1. **Data Collection**:
   - Collected information from Rappler articles related to "Marcos year 2022."
   - Downloaded the first ten pages of search results and extracted titles, links, publication dates, and snippets.

2. **Data Processing**:
   - Applied Bag of Words model to convert text into numerical features.
   - Used TF-IDF to distinguish the importance of words in the documents.
   - Implemented Latent Semantic Analysis (LSA) to identify patterns and relationships.
   - Used K-Means clustering to categorize the themes into coherent groups, evaluated using silhouette method and Calinski-Harabasz index.

![Data Processing](Data_Processing.png)

## Actionable Insights

In the political arena, the year 2022 is a turning point in the transition of presidential powers from one administration to another. Therefore, it is expected that election-related news will have its own cluster in the list of articles in our corpus given the exemplar "Marcos year 2022." This boils down to one of the clusters related to political alliances and dynasties. However, the second cluster has ties again with elections tackling the connection of media and disinformation with the exemplar.

With k=3 as the optimal number of clusters, two of the clusters are not directly associated with policies and programs. Thus, the stakeholder may only refer to the third cluster in terms of policy analysis and development. The researchers selected a few of the keywords from this cluster as a baseline for the insights on policy making.

![Actionable Insights](Actionable_Insights.png)

## Conclusion

Using Latent Semantic Analysis (LSA) to analyze Rappler news articles, this study has identified key themes and narratives surrounding President Bongbong Marcos' first year in office. The three identified clusters - "Political Alliances and Dynasties," "Media and Disinformation," and "International Relations and Economic Policies" - provide a multifaceted view of the current political and economic climate. The insights offer an assessment of the administration's image and actions, valuable for crafting strategies for policy analysis, public relations, and speech building.

## Additional Resources

- **Jupyter Notebook**: The detailed analysis and code used in this study are available in the `Shaping_Presidential_Policies_Using_Rappler_Articles.ipynb` file.
- **Technical Report**: An HTML version of the technical report can be found in the `Shaping_Presidential_Policies_Using_Rappler_Articles.html` file.

## Citation

If you use this notebook or any part of this study, please cite:

Gabriel Marco Mercado, Paul Wilhelm Nepomuceno, John Cris Orenday, Andro Cabico, "Shaping Presidential Policies Using Rappler Articles," 2024.