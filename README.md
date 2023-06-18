# history-of-neural-networks
The history of neural networks from McCulloch and Pitts to Transformers and Large Language Models, with a focus on architecture.


# Motivation
As a cognitive scientist, I write research papers on neural networks applications for an interdiscipinary audience. Some readers are intimately familiar with the history and mathematics of neural networks, while many others, particulary in the non-technical social sciences, only understand them from a functional an experiential level ― from using publicly available AI chat bots like ChatGPT.  

Every time I write a new research paper for a new audience I find my self rewriting the history section and struggling with how much detail to put into the section. Through trial and error, the best approach I've found to writing a brief history of neural networks for a diverse audience is to start with McCulloch and Pitts (1943) model of neurons, to trace the architectures that have evolved, and to note the applications of those architectures. The idea is to start with  the perceptrons of Rosenblatt (1958), to the feed-forward networks with a single hidden layer from the UCSD Parallel-Distributed Processing group (Rumelhart, Hinton, and Williams, 1985), to the multiple-hidden layer, deep learning network of Hinton, Osindero, and Teh (2006), and ending with the transformers of Vaswani et al (2017).


# A Brief History of Neural Networks 

The history of neural network starts with McCulloch and Pitts (1943), who described a mathematical model for an artificial neuron and provided a mathematical proof that a network of artificial neurons, hereafter "nodes", could perform any logical operation and, therefore, theoretically any computation. Their work laid the foundation for later research in artificial neural networks. 

The first implementation of a neural network is credited to Rosenblatt (1958). Rosenblatt named his network a "perceptron," and it consisted of two layers: an input layer and an output layer. Each node in the input layer was connected to every node in the output layer. The output nodes took the inputs, weighted them, summed the weighted inputs, and produced a result if the weighted sum exceeded a threshold. Essentially, each output node performed a task similar to linear regression, with the weights analogous to the coefficients in a regression equation. A perceptron could learn by adjusting the weights of the output nodes, akin to how one fits a regression model by modifying coefficients. Applications of perceptrons include pattern recognition tasks, such as image recognition, and learning linear functions. However, the perceptron's major drawback is its inability to handle non-linear input-output mappings, which many real-world tasks require. As a result, it cannot solve non-linear classification and regression tasks.

The inability to learn non-linear classification tasks, along with the difficulty of programming perceptrons to learn, slowed research in neural networks until the mid-80s. It was then when the Parallel Distributed Processing (PDP) group at the University of California introduced a three-layer network ― consisting of an input layer, a hidden layer, and an output layer ― and a learning algorithm known as backpropagation (Rumelhart, Hinton, and Williams, 1986). The inclusion of a hidden layer, combined with the backpropagation learning algorithm, enabled artificial networks to solve non-linear classification problems. Applications of 3-layer neural networks include image recognition, e.g., classifying images into faces or objects, speech recognition, e.g., converting spoken language to text, natural language processing, e.g., language translation, and machine learning from data, e.g. predictive models. However, there were several drawback to three-layer networks: lengthy training times, inadequate availability of big data for training, and the fact that classification algorithms like support vector machines and decision trees were more accurate.

The limitations of 3-layer networks were addressed by the introduction of networks with multiple hidden layers, known as _deep learning networks_ or _deep learning models_. These models are characterized by their depth, which refers to the number of layers between the input and output layer. The advent of big data, advancements in computing power (especially GPUs that allow the training of many artificial neurons in parallel), improved learning algorithms, and the ability to effectively train these deeper networks have together allowed deep learning to achieve performance and accuracy that often exceed those of traditional machine learning algorithms. Hinton, Osindeor, and Tech (2006) are often credited with advancing the deep learning network revolution. 


# References

Hinton, G., Osindero, S., & Teh, Y. (2006). [A fast learning algorithm for deep belief nets](https://github.com/professorf/history-of-neural-networks/blob/master/papers/Hinton-Osindero-Teh-2006.pdf). _Neural computation_, _18_, 1527-1554.

McCulloch, W. S., & Pitts, W. (1943). [A logical calculus of the ideas immanent in nervous activity](https://github.com/professorf/history-of-neural-networks/blob/master/papers/mcculloch-pitts-1943.pdf). _The bulletin of mathematical biophysics_, _5_, 115-133.

Rosenblatt, F. (1958). [The perceptron: a probabilistic model for information storage and organization in the brain](https://github.com/professorf/history-of-neural-networks/blob/master/papers/rosenblatt-1958.pdf). _Psychological review_, _65_, 386-408.

Rumelhart, D., Hinton, G., Williams, R. (1986). [Learning internal representations by error propagation](https://github.com/professorf/history-of-neural-networks/blob/master/papers/Rumelhart-Hinton-Williams-1986.pdf). In D. Rumelhart & J. McClelland (Eds.), _Parallel Distributed Processing: Explorations in the Microstructure of Cognition. Vol. 1: Foundations_ (pp. 318-362) .
Cambridge, MA: Bradford Books/MIT Press.

Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A. , ... & Polosukhin, I. (2017). [Attention is all you need](https://github.com/professorf/history-of-neural-networks/blob/master/papers/vaswani-et-al-2017.pdf). _Advances in neural information processing systems 30, 31st Conference on Neural Information Processing Systems (NIPS 2017)_, Long Beach, CA.

