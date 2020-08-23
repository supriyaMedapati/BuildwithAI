# BuildwithAI

## Introduction
* BuildwithAI Hackathon - This is the first prize Winning Natural Language Processing hack by our team - Infodemic warriors.
* Please note that the code may be messy becaues the code being written in a fast paced manner in this time-bound hackathon.
* Presentation - https://drive.google.com/file/d/1NTB3ZJe3w0d92i9Lui9jZgRAeabeNcE_/view
* Video - https://www.youtube.com/watch?v=nKwbIXTixSg


## Problem statement - What is in a tweet?
We are fighting an infodemic in the midst of a pandemic.
* In these times of fear, panic, and anxiety surrounding COVID-19, general public turns to social media to communicate their opinions, express emotions and get information.
* There is an increased information sharing without validating its authenticity and accuracy.
* At a time when reliable information is key to public health, proliferation of misinformation, pseudo-scientific news and fake news is sometimes spreading faster than the facts

## Solution
Utilize Natural Language Processing (NLP) to assess the tweets of media and influential personalities and how it influences public sentiment

Understand public perception and the influence of misinformation on public sentiment to
* Help Policymakers with data-driven decision making to introduce checks and balances to curb the spread of misinformation
* Inspire Media and influential personalities to be cognizant of their influence and share the right news
* Wake-up General Public to be more conscious about their news consumption.

## Process
* Scope and Use Case Definition
* Data gathering
* Data pre-processing
* Analyzing data for sentiment
* Data Visualization using Tableau
* Insight Gathering

## Scope
* US data only - Analysis is focused on US only due to ease of gathering data and the number of media/influential personalities information we could gather
* Twitter only - We contemplated using twitter data as well as web articles but due to retweets, it is easier to gather public opinion on tweets rather than web articles
* Duration 1 month - We initially planned to conduct the analysis from Mar-Jul 2020 but due to the time taken for hydration, we are sticking to one month data (Jun 20-Jul 20, 2020)

## Data Gathering
We collected datasets under two categories in the Date range (26 June 2020 - 25 July 2020):
* Public Tweets - For analyzing public sentiment
* Media/Influencers Tweets - For analyzing media/influencers sentiment
  * Top US Media twitter handles - categorized by political sentiment and factual correctness. Ref: mediabiasfactcheck.com
  * Public health officials - Fortune's list of trustworthy health officials.

## Data Pre-processing
Tweet IDs collected from zenodo dataset were hydrated
Removed #hashtags and urls
Performed
* Tokenization
* Punctuation
* Removal of stopwords
* Abbreviation expanding
* Stemming
* Correction of spellings

## Data analysis
* We identified key global events, public fears and conspiracy theories during the time frame of June 26, 2020 to July 27, 2020
  * Global Events: Trump supporting and wearing a mask publicly
  * Public Fears: Mental health, post COVID-19 lifestyle
  * Conspiracy theories: 5G linked to COVID-19 and conspiracy around Bill Gates
* Prepared Topic query phrases and words
* Generated BERT sentence embeddings for both tweets and topic queries
* Performed Semantic Search of tweets by estimating their Cosine similarities.
* Tweets with similarity scores greater than 0.4 to the embedding query are considered belonging to the topic.
