# Big-data-analytics
it contains research related to the application of Big Data analytics and Machine learning for the prediction of the smart grid stability

## Background information about the smart grid system
The smart grid system requires information about the consumer demand and the amount of the supplied energy, as well as the estimated grid stability to create new pricing for each energy unit sustainability of the smart grid system. Our research aims to predict and analyze the changes in energy production and consumption relative to the energy prices in a decentralized smart grid system, by performing BDA for a large dataset. To identify the grid stability for the distributed smart grid system, a mathematical model was presented in (Schäfer et al., 2016) for a four-node star architecture, with one energy source supplying three consumption nodes as displayed in , the model considers
three input features; total power balance, energy price elasticity, and response time to price changes as shown below in figure 1



<img src="https://github.com/Omarelfarouk90/Big-data-analytics/assets/53394104/5ab0602a-e80b-4c20-aeab-a9ff9803da7f" width="500" height="500">


Figure 1: Descriptive diagram for a 4 node star architecture in a smart grid system

## Steps of the Big data analytics 








<img src="https://github.com/Omarelfarouk90/Big-data-analytics/assets/53394104/7f744890-a879-4118-bacf-6c6138b0360d" width="600" height="800">


Figure 2: Steps of predicting the smart grid stability for large data analytics



Choosing the feature input and output for the machine learning model:
To identify the stability of the smart grid system, the list of inputs was identified as predictive features, they contain the following dataset 
Input features:
1.	'tau1' to 'tau4': the reaction time of each network participant, a real value within the range 0.5 to 10 ('tau1' corresponds to the supplier node, 'tau2' to 'tau4' to the consumer nodes);
2.	'p1' to 'p4': nominal power produced (positive) or consumed (negative) by each network participant, a real value within the range -2.0 to -0.5 for consumers ('p2' to 'p4'). As the total power consumed equals the total power generated, p1 (supplier node) = - (p2 + p3 + p4);
3.	'g1' to 'g4': price elasticity coefficient for each network participant, a real value within the range 0.05 to 1.00 ('g1' corresponds to the supplier node, 'g2' to 'g4' to the consumer nodes; 'g' stands for 'gamma');
Output of the machine learning model:
4.	'stab': the maximum real part of the characteristic differentia equation root (if positive, the system is linearly unstable; if negative, linearly stable);
5.	'stabf': a categorical (binary) label ('stable' or 'unstable').


Model fitting and analyzing the prediction accuracy:
Four machine learning models have been provided, the first model is related to the classification model, where the aim was to identify if the smart grid system will be considered stable or not, three machine learning models were provided using a decision tree and random forest classifier and conventional neural network (Deep learning). The fourth machine learning model was using a penalized linear regression for the prediction of the stability differential root equation.
Decision tree algorithm:
The decision tree is the usage of nodes and branches to learn the model and identify the fitness accuracy, the difference between the decision tree and the random forest is the complexity of nodes and branching.

Random forest algorithm:
Random forest algorithm is composed of different decision trees using the same node, the optimal solution is provided through the merging of various decision trees as illustrated in figure 3




<img src="https://github.com/Omarelfarouk90/Big-data-analytics/assets/53394104/009f0ac7-9f15-4fe4-a146-07f8ee0f7907" width="600" height="600">

Figure 3: Diagram showing the random forest algorithm structure used for smart grid big data analytics.

## Deep learning algorithm implemented on the smart grid system

Deep learning is a subfield of machine learning that utilizes the artificial neural network methodology to enhance model learning and data fitting.
The deep learning equations 

the neural network is a multiple layer perception consisting of various layers with each layer contains various neurons as shown in figure 4, the layers are divided into: 
input layers representing the number of variables, 12 neurons
output layer represents the number of output classification  2 neurons
hidden layers are intermediate layers used to model the decentralized smart grid system accurately, 
the first layer contains 5 neurons and the second layer contains 4 neurons.




<img src="https://github.com/Omarelfarouk90/Big-data-analytics/assets/53394104/1a772642-505f-432a-bd9a-fbac562ad8f1" width="600" height="600">

Link to the paper 

https://www.sciencedirect.com/science/article/pii/S2666827022000597


