# Word Embedding

## Notes on theory

1. [In-depth explanation:](https://pytorch.org/tutorials/beginner/nlp/word_embeddings_tutorial.html) How to represent a word in computer
	- Storing it as one-hot vector is storage-inefficiency and does not clearly show the relationship between words.
	
2. [Distributional semantics:](https://en.wikipedia.org/wiki/Distributional_semantics): Simply put, linguistic items with similar distributions have similar meanings.

## Codes
1. [Simple word embedding](../master/WordEmbedding.ipynb): The `nn.Embedding(2, 5)` create a random embedding matrix, with 2 is the vocab size, and 5 is the dimensionality (in this case, the number of characters). We have a dict `word_to_ix = {"hello": 0, "world": 1}` so that a word can represent an index, and that index can be look up in the embedding matrix by embeds(lookup_tensor).