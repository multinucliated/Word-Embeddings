# Word-Embeddings

fastText embedding: It is an extension of Mikolov’s
embedding [8]. The fastText approach is based on the skipgram model, where each word is represented as a bag of
character n-grams [16], [17]. A vector representation is
associated to each character n-gram; words being represented
as the sum of these representations. The word representation
is learned by considering a large window of left and right
context words. Unlike Mikolov’s embeddings, fastText is able
to provide an embedding for misspelled word, rare words or
words that were not present in the training corpus, because
fastText uses character n-gram word tokenization.

BERT embedding: Currently BERT (Bidirectional
Encoder Representations from Transformers) is one of the
most powerful context and word representations [18]. BERT
is based on the methodology of transformers and uses
attention mechanism. Attention is a way to look at the
relationship between the words in a given sentence [19].
Thanks to that, BERT takes into account a very large left and
right context of a given word. It is important to note that the
same word can have different embeddings according to the
context. For example, the word bank can have one embedding
when it occurs in the context the bank account and a different
embedding when it occurs in the context the bank of the river.
Moreover, BERT model uses word-piece tokenization. For
instance, the word singing can be represented as two wordpieces: sing and ##ing. The advantage is, that when the word
is not in the BERT vocabulary, it is possible to split this word
into word-pieces. Thus, it is possible to have embeddings for
rare words, like in fastText.


#link : https://hal.inria.fr/hal-02448197v2/document
