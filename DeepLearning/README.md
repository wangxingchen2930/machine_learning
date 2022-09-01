# Deep Learning


## CNN vs RNN vs FC layer
- CNN: usually used for extracting spatial relevance
- RNN (LSTM): usually used for extracting temporal relevance
- Fully connected layer: usually used before activation function (Softmax) in classifier

## Stochastic Gradient Descent
 
### Batch

A hyperparameter that defines the number of samples to work through before updating the internal model parameters.

- **Batch Gradient Descent**: Batch Size = Size of Training Set
- **Stochastic Gradient Descent**: Batch Size = 1
- **Mini-Batch Gradient Descent**: 1 < Batch Size < Size of Training Set

### Epoch

A hyperparameter that defines the number times that the learning algorithm will work through the entire training dataset.

- **Learning curves**: 
It is common to create line plots that show epochs along the x-axis as time and the error or skill of the model on the y-axis. These plots are sometimes called learning curves. These plots can help to diagnose whether the model has over learned, under learned, or is suitably fit to the training dataset.


## Meta-learning vs Transfer learning

- Meta learning is more about speeding up and optimizing hyperparameters for networks that are not trained at all
- Transfer learning (Domain Adaptation) uses a net that has already been trained for some task and reusing part or all of that network to train on a new task which is relatively similar

## Multitask learning vs Transfer learning

- Multitask learning: Giving a set of learning tasks, t1 , t2 , …, t(n), co-learn all tasks simultaneously. In other words, the learner optimizes the learning/performance across all of the n tasks through some shared knowledge.
- Transfer learning: Giving a set of source domains/tasks t1, t2, …, t(n-1) and the target domain/task t(n), the goal is to learn well for t(n) by transferring some shared knowledge from t1, t2, …, t(n-1) to t(n). Note that the goal of transfer learning is to learn well only for the target task. Learning of the source task(s) is irrelevant.

## Split learning vs Federated learning

- Federated learning: Nets trained at Clients; Merged at server

- Split learning: Nets split over network; Trained at both


## Great Learning Resource for Deep Learning

Dive into Deep Learning: http://d2l.ai/index.html

Some contents in this section borrow from it.

## Acknowledgements

Partly borrowed from Prof. Avi Kak and Prof. Charles Bouman's ECE 695DL.

Partly borrowed from Prof. Hashemi's ECE 695ODL.

