---
editor_options: 
  markdown: 
    wrap: 72
---

# topic-model

#### Group 9 Author: "Lintong Li, Jiahao Liu, Zijia Wang, Kaiwei Xiao"

#### **Introduction**

This is the report which is aimed at analyzing the most common words
from IMDB reviews, and then trying to estimate the types of movies among
these reviews.

#### Package Used
tidyverse

tidytext

janeaustenr

stringr

ggplot2

topicmodels

tm

#### Methodology
First, we plot the distribution of term frequency which is larger than
0.1, and we found that there is a very long tail to the right of this
novel which means existing those extremely rare words!

Then we use the idea of tf-idf is to find the important words for the content of
each document by decreasing the weight for commonly used words and
increasing the weight for words that are not used very much in a
collection or corpus of documents. Calculating tf-idf attempts to find
the words that are important (i.e., common) in a text, but not too
common. 

Moreover, we use the ggraph package for visualizing our networks. We plot networks of these co-occurring words so we can see these relationships better. 

Finally, we do Latent Dirichlet allocation. The β tells us the
probability of that term being generated from that topic for that
document. It is the probability of that term (word) belonging to that
topic. Notice that some of the values for β are very, very low, and some
are not so low. Next, let's examine which topics are associated with
which description fields (i.e., documents). We will look at a different
probability for this, γ, the probability that each document belongs in
each topic.
