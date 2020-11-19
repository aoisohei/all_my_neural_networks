![](https://penseeartificielle.fr/wp-content/uploads/2019/06/compilation-r%C3%A9seaux-de-deep-learning.png)

List of all networks:

| Model  | Status de crestion |
| ------------- | ------------- |
| 1. Perceptrons (P)  | ✓  |
| 2. Feed forward neural networks (FF or FFNN)  | en cours...   |
| 3. Radial basis function (RBF)  | -  |
| 4. Recurrent neural networks (RNN)  | -  |
| 5. Long / short term memory (LSTM)  | -  |
| 6. Gated recurrent units (GRU)  | -  |
| 7. Variational autoencoders (VAE)  | -  |
| 8. Denoising autoencoders (DAE)  | -  |
| 9. Sparse autoencoders (SAE)  | -  |
| 10. Markov chains (MC or discrete time Markov Chain, DTMC)  | -  |
| 11. Hopfield network (HN)  | -  |
| 12. Boltzmann machines (BM)  | -  |
| 13. Restricted Boltzmann machines (RBM)  | -  |
| 14. Deep belief networks (DBN)  | -  |
| 15. Convolutional neural networks (CNN or deep convolutional neural networks, DCNN)   | en cours...  |
| 16. Deconvolutional networks (DN)  | -  |
| 17. Deep convolutional inverse graphics networks (DCIGN)  | -  |
| 18. Generative adversarial networks (GAN)  | -  |
| 19. Liquid state machines (LSM)  | -  |
| 20. Extreme learning machines (ELM)  | -  |
| 21. Echo state networks (ESN)  | -  |
| 22. Deep residual networks (DRN)  | -  |
| 23. Neural Turing machines (NTM)  | -  |
| 24. Differentiable Neural Computers (DNC)  | -  |
| 25. Capsule Networks (CapsNet)  | -  |
| 26. Kohonen networks (KN, also self organising (feature) map, SOM, SOFM)  | - |
| 27. Attention networks (AN)  | - |

# 1. Perceptrons (P)
#### _Notes:_ 
1. The simplest somewhat practical network has two input cells and one output cell, which can be used to model logic gates.

#### _Train processe :_
#### _Model :_ ✓ [Fully connected network without Tensorflow](https://github.com/aoisohei/all_types_neural_networks/blob/main/1_fully_connected_network_without_Tensorflow.ipynb)

# 2. Feed forward neural networks (FF or FFNN)
 
#### _Notes:_ 

2. are very straight forward - they feed information from the front to the back (input and output, respectively).

3. One usually trains FFNNs through back-propagation, giving the network paired datasets of “what goes in” and “what we want to have coming out”
 
4. The error being back-propagated is often some variation of the difference between the input and the output (like MSE or just the linear difference).

5. supervised learning
through back-propagation, giving the network paired datasets of “what goes in” and “what we want to have coming out”.

unsupervised learning
where we only give it input and let the network fill in the blanks.

#### _Train processe :_
#### _Model :_
 
# 3. Radial basis function (RBF)
1. networks are FFNNs with radial basis functions as activation functions.). Et volia. Juste on ne donne pas les noms aux autres reseaux  avec propres function activation

# 4. Recurrent neural networks (RNN)

#### _Notes:_ 

1. are FFNNs with a time twist. / FFNN avec une torsion temporelle
2. ils sont sans état; ils ont des connexions entre les passes, des connexions dans le temps.
3. Les neurones reçoivent des informations non seulement de la couche précédente, mais également d'eux-mêmes de la passe précédente. - Cela signifie que l'ordre dans lequel vous alimentez l'entrée et formez le réseau est important: le nourrir de «lait» puis de «cookies» peut donner des résultats différents par rapport à l'alimentation de «cookies» puis de «lait».
2 . Un gros problème avec les RNN est le problème du gradient de disparition (ou d'explosion) où, selon les fonctions d'activation utilisées, les informations se perdent rapidement avec le temps, tout comme les FFNN très profonds perdent des informations en profondeur.
3. Les RNN peuvent en principe être utilisés dans de nombreux domaines car la plupart des formes de données qui n'ont pas réellement de chronologie (c'est-à-dire contrairement au son ou à la vidéo) peuvent être représentées sous forme de séquence.
4. Une image ou une chaîne de texte peut être alimentée un pixel ou un caractère à la fois, de sorte que les pondérations dépendant du temps sont utilisées pour ce qui précède dans la séquence, et non en fait à partir de ce qui s'est passé x secondes auparavant. En général, les réseaux récurrents sont un bon choix pour faire avancer ou compléter des informations, comme la saisie semi-automatique.

#### _Train processe :_
#### _Model :_


# 5. Long / short term memory (LSTM)
#### _Notes:_ 

1. Les réseaux tentent de combattre le problème du gradient de disparition / explosion en introduisant des portes(gates) et une cellule mémoire explicitement définie.

#### _Train processe :_
#### _Model :_

# 6. Gated recurrent units (GRU)
#### _Notes:_ 

Bidirectional recurrent neural networks, bidirectional long / short term memory networks and bidirectional gated recurrent units (BiRNN, BiLSTM and BiGRU respectively)
Autoencoders (AE)

#### _Train processe :_
#### _Model :_
 

 
# 7. Variational autoencoders (VAE)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 8. Denoising autoencoders (DAE)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 9. Sparse autoencoders (SAE)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 10. Markov chains (MC or discrete time Markov Chain, DTMC)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 11. Hopfield network (HN)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 12. Boltzmann machines (BM)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 13. Restricted Boltzmann machines (RBM)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 14. Deep belief networks (DBN)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 15. Convolutional neural networks (CNN or deep convolutional neural networks, DCNN) 
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 16. Deconvolutional networks (DN)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 17. Deep convolutional inverse graphics networks (DCIGN)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 18. Generative adversarial networks (GAN)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 19. Liquid state machines (LSM)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 20. Extreme learning machines (ELM)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 21. Echo state networks (ESN)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 22. Deep residual networks (DRN)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 23. Neural Turing machines (NTM)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 24. Differentiable Neural Computers (DNC)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 25. Capsule Networks (CapsNet)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 26. Kohonen networks (KN, also self organising (feature) map, SOM, SOFM)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_
 
# 27. Attention networks (AN)
#### _Notes:_ 
#### _Train processe :_
#### _Model :_

