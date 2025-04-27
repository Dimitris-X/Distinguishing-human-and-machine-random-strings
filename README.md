# Distinguishing human and machine generated random strings
The aim of this project is to investigate how we can differential human and LLM generated seemingly random sequences, from machine generated ones. Consider for instance a sequence of ones and 0s, each with an equal chance of occuring. While humans can accurately balance the freqeuncy of each kind, there is a tendency to avoid long sequences, and other possible biases that set these apart. This project attempts to find a method to capture this difference can be accuratly described and quantified.
The methods used to do this include examining the entropy of a string and implementing a neural network.
## Entropy based method
For details on how this method works, refer to the notebook and powerpoint presentation
Results for the entropy based method:
This method can deduce whether a string is truly random or not mostly accurately.
By calculing the p value associated with each sequence, we can somewhat reliably check if a sequence is truly random or not.
## Neural network approach.
In this section, as simple binary classifier neural network attemps to answer this question. The model will classify a series of fixed length 150 into either truly random (0) or not (1)
Results for the neural network method:
The model does detect a difference between the two types of sequences, and achived a respectable but low final accuracy of 85%. The false positive rate is about 7%
## Conclusion
We can see that the hypothesis is indeed supported by the results obtained, as both methods managed to diffentiate between the two types of data, with varying degrees of accuracy. The entropy based method is more flexible and extendable but 
