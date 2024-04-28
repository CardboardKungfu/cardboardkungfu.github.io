This folder contains the codebase for the Stop Sign classification project.

Wolfram Mathematica is required to run the .nb files. Those files are used to synthesize the training data. Note that running all of the notebooks will create ~80,000 images (~700MB) on your system. It also takes a while (~2 hours) to run.

If the user does not have Mathematica installed, that is fine. We have included a subset of the training data in the repository so that the cnn-classifier.ipynb file can still train and run the model.

To use this subset of training data, unzip "images.zip" and "base.zip" so that the folders called "images" and "base" are in the "codebase" directory. Then, run the cnn-classifier.ipynb file. Note: The model performance will be worse than as presented due to this tradeoff.

If you wish to use Mathematica to generate the training data, delete "images.zip" and run the Mathematica notebooks in this order:
1. functions.nb
2. create-negatives.nb
3. create-positives.nb

This will create a folder called "images" in the notebook directory, with subfolders "negatives" and "positives" containing the ~80,000 synthetic training images.



