# Contrastive-Loss-and-Triplet-Loss

11/5/2022

Triplet-Loss Siamese CNN can be found in - Triplet model.ipynb

Contrastive-Loss Siamese CNN can be found in - Contrative loss final model.ipynb


Two siamese convolutional neural networks were built using contrastive loss and triplet loss on the TensorFlow's ominglot data set (a collection of 1623 unique handwritten letters from 50 languages) in an attempt to develop neural networks for one-shot classifiaction for identify if two characters are from the same language or not. Both models where trained on letters from 40 of the 50 langauges and then tested on 10 untrained langauges. 
results can be found in the report(2021-IFN680-Assignment-Two_Final). Models have been reworked since the report so results may vary.

In the report and in the coding part of this assignment we were asked to test are model on the training, test and mix of training and test data. I am aware this is not a resonable practice but it is what was asked of us.

The data was split 80% training (80% trainig, 20% validation) and 20% test.

Both Siamese CNN's used the same archetecture.
Siamese CNN with Contrastive-Loss
  - The siasmese CNN contrastive-loss function ran for 20 epochs (callback function was used with a patience of 3 for loss not changing value, not used in     this case), and a batch size of 128. 
  - In trainineg the contrastive-loss network was overfitted to the training data, with 97.61% on traiing data and 82.88% on validation data.
  - Test data accurcay was 81.74%, which is a reasonable outcome for a relitively small dataset used for one-shot classification. 

Siamese CNN with Triplet-Loss
  - The siasmese CNN triplet-loss function ran for 40 epochs (callback function was used with a patience of 3 for loss not changing value, and was used after 8 epochs), and a batch size of 192. 
  - A similare overfitting was demonstrated in to the siamese network with triplet-loss function but overall better test accuracy at 91.7%

