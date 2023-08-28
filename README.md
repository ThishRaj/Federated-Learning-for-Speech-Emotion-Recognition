# Federated-Learning-for-Speech-Emotion-Recognition

## Group Members - 
 - Upal Rakshit (20204421)
 - Thishyan Raj T (20204420)

We have replicated the paper - [Federated learning for speech emotion recognition applications](https://ieeexplore.ieee.org/abstract/document/9111050) in this project.

## Speech Emotion Recognition Network
We train a Speech Emotion Recognition Network with the following architecture:

<img src="https://github.com/ThishRaj/Federated-Learning-for-Speech-Emotion-Recognition/blob/main/Architecture-FLSER.png" alt="Results" style="height: 480px; width: 960px;"/>

We use Federated Averaging algorithm to train the model in a decentralized fashion and aggregate the weights using

$w_{t+1} = \sum_{k \in S_t} \frac{n_k}{m_t} w^k_{t+1}$  

where $S_t$ is the set of all clients, $m_t$ is the number of samples in the $t$ th update, $n_k$ is the number of samples in the client during the $k$ round and $w^k_t$ is the weight update at the $t$ th update and $k$ th communication round.

## Dataset


## Results

The results are as follows:

<img src="https://github.com/ThishRaj/Federated-Learning-for-Speech-Emotion-Recognition/blob/main/Results-FLSER.png" alt="Results" style="height: 480px; width: 640px;"/>

## References -
- S. Latif, S. Khalifa, R. Rana and R. Jurdak, "Poster Abstract: Federated Learning for Speech Emotion Recognition Applications," 2020 19th ACM/IEEE International Conference on Information Processing in Sensor Networks (IPSN), 2020, pp. 341-342, doi: 10.1109/IPSN48710.2020.00-16.
- Carlos Busso, Murtaza Bulut, Chi-Chun Lee, Abe Kazemzadeh, Emily Mower, Samuel Kim, Jeannette N Chang, Sungbok Lee, and Shrikanth S Narayanan. 2008. IEMOCAP: Interactive emotional dyadic motion capture database. Language resources and evaluation 42, 4 (2008), 335.
- https://en.wikipedia.org/wiki/Federated_learning
- https://towardsdatascience.com/federated-learning-a-step-by-step-implementation-in-tensorflow-aac568283399
- Siddique Latif, Rajib Rana, Sara Khalifa, Raja Jurdak, and Julien Epps. 2019. Direct Modelling of Speech Emotion from Raw Speech. Proc. Interspeech 2019 (2019), 3920–3924.
- H Brendan McMahan, Eider Moore, Daniel Ramage, Seth Hampson, et al. 2016. Communication-efficient learning of deep networks from decentralized data. arXiv preprint arXiv:1602.05629 (2016).
