# Milestone 1: Hand in the baseline system and translation  [Report]
TEAMNAME team:
 * @github_profile_1
 * @github_profile_2
 * @github_profile_3
 
(provide links to your github profiles only)

## Our project board:
(__Screenshot__ of your project board with tasks is here; keep it __compact__ please)

## This milestone tasks description:
### Corpus Preparation
Starting from raw data, we applied following preprocessing steps:
* corpora concatenating (__link__ to github SLURM script/s): we got one big parallel text corpus of __N__ lines 
* data shuffling (__link__ to github SLURM script/s): to feed sentences to NMT system later in the random order  
* data splitting (__link__ to github SLURM script/s): __X__ training examples, __Y__ test examples, and __Z__ development examples

... 

... (__fill in here__)

* BPE (__link__ to github SLURM script/s): we used joint vocabulary of size __N__

We used [Moses](http://www.statmt.org/moses/) scripts to do basic preprocessing, and [BPE](https://github.com/rsennrich/subword-nmt) for the subword segmentation. 

### Model Training
We used 1 Tesla P100 GPU Machine provided by [HPC center of the University of Tartu](https://www.hpc.ut.ee/en_US/web/guest/home) to train our model with vocablary of size __N__. The model we trained is the default [OpenNMT-py](https://github.com/OpenNMT/OpenNMT-py) model, which consists of a 2-layer LSTM with 500 hidden units on both the encoder/decoder.

We had trained our best model for ~__N__ days, __M__ epochs. Development set perplexity was __X__. We __performed early stopping / waited to the end__ to stop the training process. You can find the script we used to run training here (__link__ to SLURM script).

### Translating and Evaluating Results
We performed an inference and got unpostprocessed English hyps file. 

We used this file, processed reference file, and BLEU metric to evaluate the translation performance of our model, and got __X__ points.

_________________________________________________________________________________________________________________
For the next milestone, we will focus on some more advanced evaluation and error analysis technics.    
