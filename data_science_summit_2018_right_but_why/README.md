# Right, but Why?!
![THINKING](https://image.ibb.co/nntWFy/Screen_Shot_2018_05_27_at_20_00_32.png)

This was a 3 hours workshop on machine learning model interpretation conducted on May 27, 2018 in the [Data Science Summit 2018 Workshop day in the IDC, Herzliya](https://events.bizzabo.com/DataScienceSummit2018/agenda/speakers/264987).
## Authors
* First Session: Hanan Shteingart, PhD
* Second Session: Yigal Wienberger

# Table of Content
A. Interpretable Models, by Hanan Shteingart, PhD
  1. [Introduction slides](decks/Right%20by%20Why_%20-%20Introduction.pdf) - talks about the motivation for this workshop: when you want to be able to understand why the model has predicted what ever it has predicted.
  2. [Naive Bayes notebook](notebooks/naive_bayes/naive_bayes.ipynb) - a naive bayes multinomial classifier interpretation example on a newsgroups 20 dataset. It shows how one can easily compute $P(class=c|feature x_i)$ thus marking words supporting the true and predicted classes.
  3. [Tree Ensemble notebook](notebooks/random_forest/random_forest.ipynb) - random forest is commonly regarded as blackbox. This is false. One can use decision paths in order to learn about the contribution of each feature to the final decision. I will show how this method can be used on the iris data set. 
  4. [Linear pitfalls notebook](notebooks/linear/linear.ipynb) - many believe a linear model is easily interpertable. However, linear coefficient are far from intuitive. Specifically, coefficient are sensitive to scaling. However, even if you normalize your features, due to mulitcolinearity, features which are positively correlated with the class may end up having a negative coefficient and vice versa. I show how can the importance of each feature can be estimated using bootstrap shuffeling. 

B. Black Box approach using LIME, by Yigal Wienberger
  1. Deck: [Peering into the blackbox](/decks/Peering%20into%20the%20black%20box.pptx)
  2. notebooks: 
      1. [MI as the product](notebooks/Peering%20into%20the%20black%20box/MI%20as%20the%20product.ipynb)
      2. [MI for Ethics](notebooks/Peering%20into%20the%20black%20box/MI%20for%20Ethics.ipynb)
      3. [MI for model improvement](notebooks/Peering%20into%20the%20black%20box/MI%20for%20model%20improvement.ipynb)
