# NLP
Create 2-gram and 3-gram character-level language models with Feed Forward Neural Network

Dataset:
● Names dataset:
○ Dataset consists of the most common 32K names taken from ssa.gov for
the year 2018.
○ Link: https://www.dropbox.com/s/6vnpqv5cacgljs0/names.txt?dl=0
○ Example:
■ zhiheng
■ ziaan
■ zichen
■ zidon


Implementation:
● Pre-process the data and append full stop at the end of every name
● Input to the network consist of character n-grams
● The model is trained to predict next character given input n-gram
● For example, if the input is “zidon.” then the training set consists of following
pairs (if the input is 2-gram)
○ zi -> d
○ id -> o
○ do -> n
○ on -> .
● The vocabulary consists of every unique character in the dataset
Input to the Neural Network:
● Input to the NN should be one-hot encoding of input tokens 
● For example, given the following name:
zidon.
● Vocabulary size: 27 (26 characters and full stop)
● The one-hot encoding for the characters is as follows:
z: [1, 0, 0, 0, 0, 0, 0, 0, …, 0]
i: [0, 1, 0, 0, 0, 0, 0, 0, …, 0]



● The dimensionality of input: [2 x 27] (in case of 2-gram) or [3 x 27] (in case of
3-gram)
● Note: You can also introduce a batch dimension
● Since the network takes a fixed length input (2 in case of 2-gram and 3 in case of
3-gram), no need to PAD the corpus.
Feed-Forward NN:
● Explain and draw the architecture of Feed-Forward NN that you are proposing
with justification. Describe the features of Feed-Forward NN.
● Network should contain TWO hidden layers
○ input — hidden_layer_1 (hidden_layer_1 size is 128)
○ hidden_layer_1 — hidden_layer_2 (hidden_layer_2 size is 64)
● Finally, hidden_layer_2 — Output (Output size is 27 as the model needs to
predict any one of the character from the vocabulary)
● Use non-linearity of your choice (tanh, relu, gelu etc.) between hidden layers
