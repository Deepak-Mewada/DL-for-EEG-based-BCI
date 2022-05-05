# Chapter3 : Deep Learning Foundations

DL is a class of ML techniques that uses many layers of information-processing stages in hierarchical architectures for pattern classification and feature/represenation learning.

### 3.1 Discriminative DL Models: are able to adaptively learn discriminative features by non-linear transformation and classification through probabilistic prediction.
                         - Ex:MLP,RNN,CNN
                         - aim is to learn a function with the mapping : x-> y.      
#### 3.1.1 MLP: One of th simplest and the most basic deep learning models,is based on the std neural network.
               -The key difference between MLP and the standard neural network is that MLP has more than one hidden layers. 
               -MLP is subset of DNN. While DNN can have loops and MLP are always feed-forward
               T(x)=wX+b;Xh1=sigma(T(x));Xh2=sigma(T(xh1));y'=sigma(T(x(h2)));error=||y'-y||2
               Afterwards the error will be backpropagated and optimized by a suigtable optimizer. 
               The optimizer will adjust all the weights and basis in the model untill the error converges. 
               loss function: cross-entropy,nrg loglikelihood,mean square
               Optimizers: Adam,SGD,Adagrad
#### 3.1.2 RNN : RNN is a subcategory of descriminative deep learning model designed to capture temporal dependencies among input data. 
                The hidden state Ct-1 can be regarded as the "memory" of the nodes which help the RNN "remember" the historical input.
                -Cells in RNN are equivalent to nodes in MLP. 
###### 3.1.2.1 LSTM             LSTM are designed to overcome the long term dependency problem/vanishing grafdient problem.

### 3.2 Representative Models: learns the pure and representative features from the input data. 
                       - Ex:DAE,RBM,DBN
                       -
                       
### 3.3 Generative Models: Which learns the joint prob. distributiuon of of the input data and the target label. VAE, GANs.
Hybrid: representation learning for deature extraction and discriminative algorithms for classification.


