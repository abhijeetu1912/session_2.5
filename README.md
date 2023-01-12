# Steps in code

1. Download train & test mnist data.
2. Create custom data generator class which returns image, label, random number and sum = label + random number. Images are normalized.
3. Create neural network class with 3 convolution layers, 1 dense layer & 2 output layers to predict label & sum respecitvely. Cross entropy loss is used for both label & sum as they are assumed to be class variable. Adam optimizer with learning rate of 1e-3 is used.
4. Initialise the model, transfer it to gpu and then train it. Calculate total loss as sum of loss from both label & sum.
5. Evaluate model by claculating accuracy for both label & sum on both train & test data.


# Training log

Epoch 0: | Train Loss: 1.64804 | Test Loss: 2.52513 \
Epoch 1: | Train Loss: 0.20629 | Test Loss: 0.54847 \
Epoch 2: | Train Loss: 0.09629 | Test Loss: 0.40790 \
Epoch 3: | Train Loss: 0.07404 | Test Loss: 0.31103 \
Epoch 4: | Train Loss: 0.06020 | Test Loss: 0.30970 \
Epoch 5: | Train Loss: 0.04956 | Test Loss: 0.24033 \
Epoch 6: | Train Loss: 0.04338 | Test Loss: 0.17115 \
Epoch 7: | Train Loss: 0.03997 | Test Loss: 0.14499 \
Epoch 8: | Train Loss: 0.03771 | Test Loss: 0.16685 \
Epoch 9: | Train Loss: 0.03233 | Test Loss: 0.20463 


# Model performance 

Accuracy on Train Data - Label:  0.996 \
Accuracy on Train Data - Sum:  0.993 

Accuracy on Test Data - Label:  0.992 \
Accuracy on Test Data - Sum:  0.99
