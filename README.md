# Meme_analysis_challenge
My solution to Kaggle Meme Analysis Challenge

I've divided this fun project into three parts: 
a. ML algorithm that will do hateful/not-hateful meme classification based only on texts extracted from memes;
b. ML algorithm that will do hateful/not-hateful meme classification based only on meme images;
c. design a joint algorithm that uses learned information from images+texts.

I've used different ML approaches (classical and deep learning) but got the best results when:
a. gensim FastText embeddings are used for the text;
b. VGG-type CNN is used on resnet_v2 preprocessed images;
c. then the results are concatenated with a simple NN over it. 

I've got cross-validated 75% accuracy using this approach, which is rather cool, as used technics are extremely simple and easily reproducible. 
