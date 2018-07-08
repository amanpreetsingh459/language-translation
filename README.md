# language-translation

This repository contains the code for a sequence to sequence deep learning model that has been trained on a data set of English and French sentences. It can translate new sentences from English to French with 90 per cent accuracy.

## Files and folders into the repository : -
* ### dlnd_language_translation.ipynb
This notebook contains the actual code for the whole project to implement seq-to-seq model
* ### dlnd_language_translation.html
This is the equivalent html file for the notebook. This has been included for having the quick look on any of the portion of whole code in simpler format.
* ### Data
Since translating the whole language of English to French will take lots of time to train, so a samll portion of data is included in the repository upon which the model can be trained. Two different files contains small corpus for english and french datasets in the "data" directory.
* ### helper.py
This python file contains the code for helper functions which are used for various tasks such as 'loading data' and 'pre-processing' the data and batching.
* ### problem_unittests.py
This python files contains code to perform unit tests for the code which we have written. This is good way to verify the code after each meaningful step.
* ### preprocess.p
This file contains the preprocessed data which contains the values for the various python objects which we created during the development of the code. This helps in loading the data multiple times from the previously saved objects. Thus we do not need to process them again.

#### Below is the translation done by our created model
<img src="/assets/images/img1.jpg">

#### Below is the translation what google translator does
<img src="/assets/images/img2.jpg">

## Imperfect Translation
You might notice that some sentences translate better than others.  Since the dataset we're using only has a vocabulary of 227 English words of the thousands that we use, we're only going to see good results using these words. However, if you want to create a better translation model, you'll need better data.

You can train on the [WMT10 French-English corpus](http://www.statmt.org/wmt10/training-giga-fren.tar). This dataset has more vocabulary and richer in topics discussed. However, this will take you days to train, so make sure you've a GPU and the neural network is performing well on dataset we provided.

### Dependencies
The code uses tensorflow 1.0 or later version.

### Good luck...
