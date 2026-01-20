# Latent Variable Energy-Based Model for Handwriting Recognition
## Using a Latent Variable Energy-Based Model for Handwriting Recognition. This tiny project followed as a personal proof-of-concept after a series of lectures by Yann LeCun and Alfredo Canziani on LV-EBMs. 
## This work was planned by me, in terms of architectural design choices, and general logical flow.
## However, I employed the help of Gemini to write the Syntax.

### This tiny project demonstrates the use of Latent Variable Energy-Based Model to do Handwriting Recognition.
### It goes a step further from ordinary classification to deciding where the boundaries of characters(digits) are in a multiple-digit image sample.
### The Latent Variable in this problem is taken to be the pixel indicating the cutting position of a two conjoined MNIST image data.
### We start by making an informed guess during Inference to determine a 'good enough' Latent Variable (z). 
### Then we use an untrained judge (a simple CNN) to identify the characters.
### Next we calculate the energy between the z and the result.
### We use this result to update the weights of the untrained CNN.
### We end up achieving the dual goal of picking the best z and training a good classification model.
