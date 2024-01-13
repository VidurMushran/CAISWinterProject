# CAISWinterProject

Vidur Mushran
mushran@usc.edu

I finetuned DistilBERT on a database of Sarcastic vs Normal text. They used News Headlines fetched from the Onion (sarcastic), and HuffPost (normal), as fetching tweets based on hashtags is too noisy as many users don’t tag their tweets knowing that in context their audience will infer the sarcastic tone. For preprocessing as it was a NLP task, I had to tokenize the dataset, and split it into a train and test set. For model architecture I stuck to the lesson 4 notebooks style, using BERT and Adam for my optimizer. As for hyper parameter training, I stuck to the default 0.001 learning rate for Adam. When I set it on a learning rate of 0.01 it looked like it was having a lower training loss and higher accuracy after the first 2 epochs but my connection quit and I didn’t want to wait through another hour of training because I was rushing this project out a bit. I did pillage the hyperparameter training code from hugging face’s Text Classification on GLUE sample notebook but it involve installing a couple packages & would take a while. I did want to try DistilBERT after training BERT in the hopes that it would train faster due to it’s smaller size while hopefully retaining much of the performance. As for Model evaluation, I just used the same exact metrics as the initial BERT notebook 4 so I only had positive samples and the epoch statistics. Unfortunately Validation Loss and accuracy didn’t improve at all during this training session so I should increase the learning rate. As I mentioned before I definitely want to try DistilBERT as it will train faster and I would want to adapt the hyperparameter code to this project if I were to continue.


Positive samples: 13634 of 28619 (47.64%)
