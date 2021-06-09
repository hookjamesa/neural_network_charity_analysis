# neural_network_charity_analysis

## Overview

The purpose of this analysis is to identify reliable predictors for whether or not applications to AlphabetSoup (a made up charity for these purposes) will be successful, and to train a simple neural network to reliably predict application success.

## Analysis

The following variables are considered targets for the model: 'IS_SUCCESSFUL'. The primary features for this model are: 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT', and 'SPECIAL_CONSIDERATIONS'. I believe that 'AFFILIATION','USE_CASE', and 'ORGANIZATION' can likely be removed from the features list.

Despite the model not achieving 75% accuracy, several attempts were made to try to increase the initial 72.4% accuracy higher. These attempts included adding an additional neuron layer, changing the activation function to 'softmax' for the second and third layers to provide a probability distribution, and changing the number of neurons in each layer. The next attempt to change the model accuracy would be to remove noisy variables from consideration.

## Results

The initial model with two layers - 8 and 5 neurons respectively - was the best accuracy obtained at 72.4%. Given the relatively discrete values given in several lines, including 'INCOME_AMT', I believe that a random forest model may be a better model, as it would be easier to explain to those less technical.
