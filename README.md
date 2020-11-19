# 1. All types Neural Networks

My reposytory has next neural networks :

✓ [Fully connected network without Tensorflow](https://github.com/aoisohei/all_types_neural_networks/blob/main/1_fully_connected_network_without_Tensorflow.ipynb)

![](https://penseeartificielle.fr/wp-content/uploads/2019/06/compilation-r%C3%A9seaux-de-deep-learning.png)


List of all networks:

Perceptrons (P)

    
1. The simplest somewhat practical network has two input cells and one output cell, which can be used to model logic gates.
 

Feed forward neural networks (FF or FFNN)
 

2. are very straight forward - they feed information from the front to the back (input and output, respectively).

3. One usually trains FFNNs through back-propagation, giving the network paired datasets of “what goes in” and “what we want to have coming out”
 
4. The error being back-propagated is often some variation of the difference between the input and the output (like MSE or just the linear difference).

5. supervised learning
through back-propagation, giving the network paired datasets of “what goes in” and “what we want to have coming out”.

unsupervised learning
where we only give it input and let the network fill in the blanks.

 
Radial basis function (RBF)
1. networks are FFNNs with radial basis functions as activation functions.). Et volia. Juste on ne donne pas les noms aux autres reseaux  avec propres function activation

Recurrent neural networks (RNN)
 
1. are FFNNs with a time twist. / FFNN avec une torsion temporelle
2.: ils sont sans état; ils ont des connexions entre les passes, des connexions dans le temps.
3. Les neurones reçoivent des informations non seulement de la couche précédente, mais également d'eux-mêmes de la passe précédente. - Cela signifie que l'ordre dans lequel vous alimentez l'entrée et formez le réseau est important: le nourrir de «lait» puis de «cookies» peut donner des résultats différents par rapport à l'alimentation de «cookies» puis de «lait».
2 . Un gros problème avec les RNN est le problème du gradient de disparition (ou d'explosion) où, selon les fonctions d'activation utilisées, les informations se perdent rapidement avec le temps, tout comme les FFNN très profonds perdent des informations en profondeur.
3. Les RNN peuvent en principe être utilisés dans de nombreux domaines car la plupart des formes de données qui n'ont pas réellement de chronologie (c'est-à-dire contrairement au son ou à la vidéo) peuvent être représentées sous forme de séquence.
4. Une image ou une chaîne de texte peut être alimentée un pixel ou un caractère à la fois, de sorte que les pondérations dépendant du temps sont utilisées pour ce qui précède dans la séquence, et non en fait à partir de ce qui s'est passé x secondes auparavant. En général, les réseaux récurrents sont un bon choix pour faire avancer ou compléter des informations, comme la saisie semi-automatique.

Long / short term memory (LSTM)

 

1. Les réseaux tentent de combattre le problème du gradient de disparition / explosion en introduisant des portes(gates) et une cellule mémoire explicitement définie.

Gated recurrent units (GRU)
 
Bidirectional recurrent neural networks, bidirectional long / short term memory networks and bidirectional gated recurrent units (BiRNN, BiLSTM and BiGRU respectively)
Autoencoders (AE)

 
Variational autoencoders (VAE)
 
Denoising autoencoders (DAE)
 
Sparse autoencoders (SAE)
 
Markov chains (MC or discrete time Markov Chain, DTMC)
 
Hopfield network (HN)
 
Boltzmann machines (BM)
 
Restricted Boltzmann machines (RBM)
 
Deep belief networks (DBN)
 
Convolutional neural networks (CNN or deep convolutional neural networks, DCNN) 
 
Deconvolutional networks (DN)
 
Deep convolutional inverse graphics networks (DCIGN)
 
Generative adversarial networks (GAN)
 
Liquid state machines (LSM)
 
Extreme learning machines (ELM)
 
Echo state networks (ESN)
 
Deep residual networks (DRN)
 
Neural Turing machines (NTM)
 
Differentiable Neural Computers (DNC)
 
Capsule Networks (CapsNet)
 
Kohonen networks (KN, also self organising (feature) map, SOM, SOFM)
 
Attention networks (AN)
 

