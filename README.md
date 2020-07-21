# Aspect-based-Sentiment-Analysis-Dataset

The purpose of this labelled dataset for aspect-based sentiment analysis is to detect aspect terms and their sentiment polarity within reviews. Customer reviews are basically the sentences of the restaurant domain which are taken from amazon. 

In a given review, the basic task is to identify the explicit aspect terms that are clearly mention in the text, the sentiment containing words/phrases and sentiment polarity of the aspect term, and also the sentiment polarity of each review is also mentioned.


Review 1: I love the food and atmosphere, but staff was incompetent

Review 2: The fries with mayo are not tasty

Review 3: My friend took me there for thai food


Aspect Term: An aspect term can be single word or multi words.  In review 1, the aspect terms are “food”, “atmosphere” and “staff”. In review 2, the only aspect term is “fries with mayo”. And in review 3, “thai food” is the aspect term.

Aspect Term Sentiment Polarity: Each aspect term is assigned one of the following polarities, positive +1, negative -1, neutral 0, based on the sentiment that is expressed in the review about it. In review 1, the aspect terms “food” and “atmosphere” have positive sentiment polarity and aspect term “staff” has negative sentiment polarity. Similarly, in review 2, the aspect term “fries with mayo” has negative sentiment polarity. In review 3, the aspect term “thai food” has neutral sentiment polarity.

Sentiment-contain word/phrases: The sentiment polarity of each aspect term as positive, negative and neutral is decided by sentiment-containing word/phrases. In review 1, the sentiment-containing word “love” decides the positive sentiment polarity for aspect terms “food”, and “atmosphere”, and sentiment-containing word “incompetent” decides the negative sentiment polarity for aspect term “staff”. In review 2, the sentiment-containing phrase “not tasty” decides the negative sentiment polarity for the aspect term “fries with mayo”. But in review 3, the reviewer does not express any sentiment about aspect term “thai food” that’s why it doesn’t contain ant sentiment-containing word/phrase, thus doesn’t hold any positive or negative sentiment and possesses a neutral sentiment polarity.

Review Sentiment Polarity: Each review has assigned one of the following polarities, positive +1, negative -1, neutral 0, based on the overall sentiment of the review. Review 1 holds a positive sentiment polarity because it’s two aspect terms “food” and “atmosphere” have positive sentiment polarity. Review 2 holds a negative sentiment polarity. And review 3 has neutral sentiment polarity.  

The information about aspect terms, aspect/review sentiment polarities and sentiment-containing word/phrases has been labelled in the dataset using the following syntax:

Review ID [review sentiment polarity]

Review Text

[aspect term, sentiment-containing word/phrase aspect term sentiment polarity] , ….



1

I love the food and atmosphere, but staff was incompetent  [+1]

[food, love +1], [atmosphere, love +1], [staff, incompetent -1] 



2

The fries with mayo are not tasty  [-1]

[fries with mayo, not tasty -1]


3

My friend took me there for thai food [0]

[thai food, 0]
