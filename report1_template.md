# Milestone 1: Hand in the baseline system and translation  [Report]
TEAMNAME team:
 * @github_profile_1
 * @github_profile_2
 * @github_profile_3
 
(provide links to your github profiles only)

## Our project board:
(Screenshot of your project board with tasks is here; keep it compact please)

## This milestone tasks description:
### Corpus Preparation
Starting from raw data, we applied following preprocessing steps:
* corpora concatenating (link to github SLURM script/s): as a result we got one big parallel text corpus of size N
* data shuffling (link to github SLURM script/s): to feed sentences to NMT system later in the random order  
* data splitting (link to github SLURM script/s): as a result we got X training examples, Y test examples, and Z development examples

...

...

...

We used [Moses](http://www.statmt.org/moses/) scripts to do basic preprocessing, and [BPE](https://github.com/rsennrich/subword-nmt) for the subword segmentation. 

### Model Training
We used 1 Tesla P100 GPU Machine provided by [HPC center of the University of Tartu](https://www.hpc.ut.ee/en_US/web/guest/home) to train our model with vocablary of size N. The model we trained is the default [OpenNMT-py](https://github.com/OpenNMT/OpenNMT-py) model, which consists of a 2-layer LSTM with 500 hidden units on both the encoder/decoder.

We had trained our best model for ~N days, M epochs. Development set perplexity was X. We performed early stopping / waited to the end to stop the training process. You can find the script we used to run training here (link to SLURM script).

### Translating and Evaluating Results
We performed an inference and got unpostprocessed English hyps file. 

We used this file, processed reference file, and BLEU score to evaluate the translation performance of our model, and got X points.

_________________________________________________________________________________________________________________
For the next milestone, we will focus on some more advanced evaluation and error analysis technics.    
