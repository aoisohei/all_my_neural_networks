# Perceptron
The simpler, somewhat practical network has two or more input cells and one output cell, which can be used to model logic gates or decision-making.
## Step 1. Input layer and Output layer
We start write with a little guess : Suppose we have three different binary conditions (yes or no) and one binary solution in the output (yes or no):

**Input layer** 
*(binary conditions)* :
1. friends wil be there = 1 0 0
2. booze = 0 1 0
3. rain = 0 0 1
    
**Output layer** 
*(solution in the output)* :
- "to be or not to be" at the party

We can show it like this :    
![](https://i.imgur.com/LWPhtci.png)
## Step 2. Hidden layer
The perceptron neural network is simply stand-alone blocks of neurons (blocks: input layer, hidden layer, output layer) interconnected. Let's create a simple neuron with a hidden layer of three neurons:
![](https://i.imgur.com/CCsRGBl.png)

## Step 2. Synapse
The synapses of the neuron in turn receive information from other neurons and therefore allow neurons to communicate with each other. That is, the neurons themselves do not decide anything at all, synapses makes the decision exactly :
![](https://i.imgur.com/W1KVXB8.png)

## Step 3. Value of input
Each input on the left has a value: 0 or 1, yes or no. Let's add these values to the input, let's say it's raining outside (rain = 1), but friends are (friends = 1) at the party :
![](https://i.imgur.com/ZOioaIV.png)

## Step 4. We set the weight at random.
1. friends wil be there = 0.9
2. booze = 0.2
3. rain = 0.2
![](https://i.imgur.com/lxugYu3.png)

## Step 5. Multiply weights by the input values
We multiply weights by the input values and for convenience, let's imagine that something can be put into neurons:
![](https://i.imgur.com/4Mq6J6x.png)

## Step 6. Then we add the values
Then we add the values (in one of the perceptron implementations):
![](https://i.imgur.com/PB3fzns.png)

## Step 6. Training
If the amount is more than 0.5, you need to go to the party. If less or equal, you don't need to go to the party. Of course, the model above is of little practical use, we need to train it. Frightening phrase "train neurons" - isn't it? Not this way. Everything is clumsy and as simple as possible: you take random data at the input (as we did), run the input through these three neurons, look at the answer - let it be positive (let's go to a party) - and check whether the neuron predicted the answer correctly or not ... If it is correct, you do nothing. If it is wrong, you slightly shift the weights of the neurons (one at a time or all at once) in any direction :
![](https://i.imgur.com/OkuT7JP.png)

## Step 7. Add new layer
Then everything is simple: instead of one layer of neurons, we make two and again we go through everything according to exactly the same principles, only all the neurons give values to other neurons. If at first we had only 3 neurons, now we have 3 + 9 neurons with weights. And then three layers, four, recursive layers and stuff like that:
![](https://i.imgur.com/yJKXP8M.png)
We have 0.475 + 0.545 + 0.61 = 1.63. We weill use it in Step 8.

## Step 8. Function activations : Softmax Function and Hyperbolic Tangent
We have 0.475 + 0.545 + 0.61 = 1.63 :

We will use \ 0.475 \ 0.545 \ 0.61 \ in Softmax Function ;

And we will use \ 1.63 \ like x in  Hyperbolic Tangent.
- ## Softmax Function
 
Formula :
![](https://i.imgur.com/tYoHtiW.png)

Use \ 0.475 \ 0.545 \ 0.61 \ in Softmax Function
```
# transform values into probabilities
from math import exp

# calculate each probability
p1 = exp(0.475) / (exp(0.475) + exp(0.545) + exp(0.61))
p2 = exp(0.545) / (exp(0.475) + exp(0.545) + exp(0.61))
p3 = exp(0.61) / (exp(0.475) + exp(0.545) + exp(0.61))

# report probabilities
print(p1, p2, p3)

# report sum of probabilities
print(p1 + p2 + p3)
```
The result of code :
```
0.3108442718990016               0.3333830247076894              0.35577270339330896
1.0
```

- ## Hyperbolic Tangent
```
x = 1.63
tanh_x_1 = exp(x) - exp(-x) 
tanh_x_2 = exp(x) + exp(-x) 
tanh_x = tanh_x_1 / tanh_x_2
tanh_x
```
0.92

The result :
tanh(x) = 0.92
randian = 0.75

<\hr>

***Read more :*** 

- *[Softmax Function with Python, Types of other functions :](https://machinelearningmastery.com/softmax-activation-function-with-python/)*

- *[Wiki, explication of Softmax Function :](https://www.google.com/search?q=function+activation+softmax&oq=function+activation+softmax&aqs=chrome..69i57.6793j0j7&sourceid=chrome&ie=UTF-8)*

- *[Hyperbolic Tangent Function](https://sefiks.com/2017/01/29/hyperbolic-tangent-as-neural-network-activation-function/#:~:text=In%20neural%20networks%2C%20as%20an,for%20error%20effects%20on%20weights.&text=In%20other%20words%2C%20function%20produces%20output%20for%20every%20x%20value) 

- *[Style of this file taken from this example](https://habr.com/ru/post/416211/)* 

# Result
Based on these functions (Softmax Function = 1, Hyperbolic Tangent = 0.92 (0.75) ).
I go to the party.

