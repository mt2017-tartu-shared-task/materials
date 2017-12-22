# __TEAMNAME__ In-class Machine Translation Shared Task 2017 Submission
This repository is a result of our participation in the shared task.<br>
We went through the process of building, analyzing, and improving the neural machine translation system.

Poster: [link]() // feel later, no need to feel now

The shared task was for Estonian-English language pair. 
It included working with ~19.000.000 sentence pairs.

Shared task main page: [link](https://github.com/mt2017-tartu-shared-task) <br>
Shared task on course page: [link](https://courses.cs.ut.ee/2017/MT/fall/Main/SharedTask)

Sections below summarize key milestones we went through.  

##  Baseline system
- Our baseline system was pretty decent.
- As a result, we got 35.97 BLEU points on the shared dev set.

More details: [link](https://github.com/mt2017-tartu-shared-task/nmt-system-F/blob/master/reports/report1.md).

## Baseline system manual evaluation
- We manually analyzed 40 baseline translations. 
- Or main observation was that the sintactic structure was not fully correct, so we tried to improve on this aspect.
- Take a look at our the motivating example produced by baseline system:
"ORIGINAL: Tests were carried out in Germany , Hungary , the Netherlands , Slovenia and Slovakia on nearly 200 sets of light strings in all price categories.<br>
TRANSLATED: The tests were carried out in Germany , Hungary , the Netherlands , Slovenia and Slovakia on a set of price categories of almost 200 sheep"

More details: [link](https://github.com/mt2017-tartu-shared-task/nmt-system-F/blob/master/reports/report2.md).

## Final system
- In order to address translation issues found after our manual evaluation we wanted to insert Standford CoreNLP. 
- The trained system gave us the same BLEU points as before as we were not able to use CoreNPL.

More details: [link report 3](https://github.com/mt2017-tartu-shared-task/nmt-system-F/blob/master/reports/report3.md).<br>
[link report 4](https://github.com/mt2017-tartu-shared-task/nmt-system-F/blob/master/reports/report4.md).

Do not forget to check our poster: [__POSTER_LINK__]

## What we also tried or wanted to try
We tried to include Standford CoreNPL. Stanford CoreNLP provides a set of human language technology tools. It can give the base forms of words, their parts of speech, whether they are names of companies, people, etc., normalize dates, times, and numeric quantities, mark up the structure of sentences in terms of phrases and syntactic dependencies, indicate which noun phrases refer to the same entities, indicate sentiment, extract particular or open-class relations between entity mentions, get the quotes people said, etc. So, with this, we wanted to fix some sintactical problems of our system. But we could not.

## Final words
- __1st_sentence: We can't compare our system before and after because sadly, there is not a before and an after.
- __2nd_sentence: Our main difficulty was the second iteration of the system as we could not improve it.
- __3rd_sentence: We have learnt that is not as easy at it looks to train a system for translation. And also that the translation world has to improve a lot yet.


## Team members:
1. https://github.com/eruizdeloizaga002
2. https://github.com/vampnik

Project board: [link](https://github.com/mt2017-tartu-shared-task/nmt-system-F).

