---
author: Imama Lavi
date: "2021-11-22"
image: Rplot01.png
title: Comparing sentiment analysis from different lexicon of Pride and Prejudice Novel
---

Working with text mining means we can dig more about what the content meaning in particular text. We can see the emotional tone that used by the author, it is positive or negative. Thus we can called opinion mining or sentiment analysis.

We know there are several methods to do the sentiment analysis but in this article we want to discuss about sentiment analysis using lexicon in tidytext package. Here are the three different lexicons based on unigrams:
1. AFINN from Finn Årup Nielsen,
2. bing from Bing Liu and collaborators, and
3. nrc from Saif Mohammad and Peter Turney.

The Bing lexicon uses a binary categorization model that sorts words into positive or negative positions.The AFINN lexicon grades words between -5 and 5 (positive scores indicate positive sentiments).The NRC lexicon categorizes sentiment words into positive, negative, anger, anticipation, disgust, fear, joy, sadness, surprise and trust.

So, let's start the code:

1. import the library

```{r, echo = TRUE}
library(tidytext)
library(janeaustenr)
library(dplyr)
library(stringr)
library(tidyr)
library(ggplot2)
```
