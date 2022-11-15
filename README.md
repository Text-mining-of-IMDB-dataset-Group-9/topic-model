---
editor_options: 
  markdown: 
    wrap: 72
---

# topic-model

##Group 9 Author: "Lintong Li, Jiahao Liu, Zijia Wang, Kaiwei Xiao"

#### **Introduction**

This is the report which is aimed at analyzing the most common words
from IMDB reviews, and then trying to estimate the types of movies among
these reviews.

#### Evaluation

First, we plot the distribution of term frequency which is larger than
0.1, and we found that there is a very long tail to the right of this
novel which means existing those extremely rare words!

The idea of tf-idf is to find the important words for the content of
each document by decreasing the weight for commonly used words and
increasing the weight for words that are not used very much in a
collection or corpus of documents. Calculating tf-idf attempts to find
the words that are important (i.e., common) in a text, but not too
common. From the tf_itf table, we know the top 10 words are
trivialboring, cognac, smallville, sandra, blahblah, amália, colombo,
tarzan.

Then, From df table and networks visulization, we know the most common
words are MOVIE, FILM, BAD, MOVIES, STORY, LOVE, FUNNY, TIME, WATCH,
SERIES. We can guess the popular movies that people like from the above
ten words. People are prone to watching story or series movies, such as
Marvel movies. Additionally, we found that people also like to watch
funny movies. The reason may be that people are busy today, and they
prefer to watching the comedies to entertainment rather than the serious
movies like documentary movies.

Finally, we do Latent Dirichlet allocation. The β tells us the
probability of that term being generated from that topic for that
document. It is the probability of that term (word) belonging to that
topic. Notice that some of the values for β are very, very low, and some
are not so low. Next, let's examine which topics are associated with
which description fields (i.e., documents). We will look at a different
probability for this, γ, the probability that each document belongs in
each topic.
