# News-Suggestor
News Suggestor is a subclass of information filtering system that seeks to predict preference a user would give to read a news article based on his current choice.  
This dataset contains around 200k news headlines from the year 2012 to 2018 obtained from HuffPost in Json format.  
Each json record contains following attributes:
{
category: Category of the article 
headline: Headline of the article
authors: author of the article
link: Link to the post
short_description: Short description of the article
date: publishing date of article
}
It can be downloded from: https://www.kaggle.com/rmisra/news-category-dataset?select=News_Category_Dataset_v2.json   
In this model based on title-title similarity, top 15 similar news headline is being suggested.  
Strategy:  
1. *Data loading* : (loading json data)  
2. *Data Cleaning* : (dedublication)  
3. *Data Prepocessing* : (removing Stopwords)  
4. *TF-IDF Vectorizer* : (to convert a collection of raw documents to a matrix of TF-IDF features)  
5. *Cosine Similarity* : (calculates similarity by measuring the cosine of angle between two vectors.)  
6. *Suggestion* : (providing top 15 suggestion based on user choice)
