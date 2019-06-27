# Word2Vec
Sample code that does Embeddings and Word to Vector learning.  There are two Jupyter Notebook files here, [Negative_Sampling_Solution.ipynb](https://github.com/the-john/Word2Vec/blob/master/word2vec-embeddings/Negative_Sampling_Solution.ipynb) and [Skip_Grams_Solution.ipynb](https://github.com/the-john/Word2Vec/blob/master/word2vec-embeddings/Skip_Grams_Solution.ipynb).

When you are working with text, there are HUGE amounts of words to analyze.  Using traditional "one-hot encode" methods proves to be very inefficient.  So, embeddings come into play.  Embeddings are a Fully Connected (FC) layer that consists of a weight matrix, that we use as a lookup table.  We encode each word as an integer, and take the that integer row from the lookup table to get your hidden layer values for the word.


The **Skip_Grams_Solution.ipynb** notebook shows sample code that shows how to implement the [Word2Vec algorithm](https://en.wikipedia.org/wiki/Word2vec) using skip-gram architecture.  The [Word2Vec algorithm](https://en.wikipedia.org/wiki/Word2vec) finds much more efficient represntations by finding vectors that represent words.  The vectors also contain semantic information about the words.  Words that show up in similar **context**, such as "coffee", "tea", and "water" will have vectors near each other.  Different words will have vectors further away from one another.  So the relationships between words can be represented by distance in vector space.  There are two architectures for implementing the [Word2Vec algorithm](https://en.wikipedia.org/wiki/Word2vec), CBOW and Skip-Gram.  CBOW = Continuouse Bag-Of-Words.  It is said that Skip-Gram performs better than CBOW.


The **Negative_Sampling_Solution.ipynb** notebook shows sample code that shows how to embedd words for use in natural language processing.  This type of code is useful when you're trying to do Machine Translation.  Here I implement the [Word2Vec algorithm](https://en.wikipedia.org/wiki/Word2vec) using the skip-gram architecture.

Some recommended reading material is:
- A [conceptual overview](http://mccormickml.com/2016/04/19/word2vec-tutorial-the-skip-gram-model/) of Word2Vec from Chris McCormick
- The first [Word2Vec](https://arxiv.org/pdf/1301.3781.pdf) white paper from Mikolov et al.
- And one other white paper [Neural Information Processing Systems](http://papers.nips.cc/paper/5021-distributed-representations-of-words-and-phrases-and-their-compositionality.pdf) from Mikolov et al.


