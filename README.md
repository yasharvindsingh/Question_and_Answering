# Question_and_Answering

A simple question and answering system using the babi tasks dataset.

Vocabulary: Since, the vocabulary for the problem has been developed from the dataset (length of vocabulary = 21) not all words or sequences will work, the vocabulary has been displayed in the ipynb file for the task.

Model: There are two major points in the model,
1) The dot product of the encoded story and question, and then concatenating the result to encoded story.
2) Passing the tensor obtained from above to LSTM, for sequence processing.

Example:

Custom input:
Story (provide spaces even before punctuation marks): John moved to the hallway . John journeyed to the kitchen . Sandra travelled to the garden . John journeyed to the garden . Daniel journeyed to the office . John went to the kitchen . Sandra journeyed to the hallway . Mary went to the hallway . Mary went to the kitchen . Sandra travelled to the garden .

Question (provide spaces even before punctuation marks): Where is John ?

predicted:  kitchen

How to run for custom input ?

Since, the model has already been trained and saved (model.h5), so the training part can be skipped. But the program demands the creation of vocabulary every time the runtime has been set. While running for custom input run all the cells, except the training (model.fit) and then provide the input in the required format.

ref: https://github.com/prashil2792/Question-Answering-System-Deep-Learning
