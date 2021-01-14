---
layout: page
title: Shared Task
permalink: /shared_task
---

## Shared Task: Predicting human reading patterns

The ability of accurately modeling eye-tracking features is crucial to advance the understanding of language processing. Eye tracking provides millisecond-accurate records on where humans look when they are reading, shedding lights on where humans pay attention during their reading and comprehension phase. The benefits of utilizing eye movement data have been noticed in various domains, including natural language processing and computer vision.
Thanks to the recent introduction of a standardized dataset, it is finally possible to compare the capabilities of machine learning approaches to model and analyze human patterns of reading. In this shared task, we present the challenge of predicting eye tracking-based metrics recorded during English sentence processing. We are interested in submissions concerning both cognitive modelling approaches and linguistically motivated approaches (e.g., language models).


### Task

The shared task if formulated as a regression task to predict 5 eye-tracking features:
1. number of fixations (nFix), total number of fixations on the current word; 
2. first fixation duration (FFD), the duration of the first fixation on the prevailing word; 
3. total reading time (TRT), the sum of all fixation durations on the current word, including regressions; 
4. go-past time (GPT), the sum of all fixations prior to progressing to the right of the current word, including regressions to previous words that originated from the current word;
5. fixation proportion (fixProp), the proportion of participants that fixated the current word (proxy for how likely a word is to be fixated).


## Links and Contacts

- For data and submission details, visit: [CODALAB, https://competitions.codalab.org/competitions/28176](https://competitions.codalab.org/competitions/28176)
- For questions, contact: [cmcl2021sharedtask@gmail.com](mailto:cmcl2021sharedtask@gmail.com)


## Timeline

- January 15, 2021: Trial data release
- January 29, 2021: Participant registration deadline & training data release
- February 23, 2021: Test data release 
- March 2, 2021: Submission deadline
- March 9, 2021: Results release
- March 22: Paper submission deadline
- April 15: Reviews released to participants
- April 26: Camera-ready papers due


## Data

We will use the ZuCo eye-tracking dataset recorded during normal reading (1000 sentences). The training data will contain approx. 800 sentences, and the test set 200 sentences. The data provided will contain normalized features (feature values between 0 and 100 to facilitate evaluation via MAE) averaged over all participants.

Example:

```
word_id	sentence_id	word	nFix	FFD	GPT	TRT 	fixProp
0	1	After	6.47	23.47	11.61	7.48	47.06
1	1	the	7.19	20.79	10.39	6.70	52.94
2	1	show	12.22	35.61	16.42	13.84	76.47
3	1	was	7.19	20.87	9.62	6.21	58.82
4	1	cancelled,	12.94	27.61	13.94	12.20	70.59
```

Note: Any additional data source is allowed, as long as it is freely available to the research community. For example, additional eye tracking corpora, additional features such as brain activity signals, pre-trained language models, etc.


## Evaluation

We will evaluate the prediction against the ground truth using the mean absolute error (MAE).
The winning system will be the one with the best average MAE across all 5 eye-tracking features.


## Papers

System description papers will be short papers (4 pages + references) describing the approach used for the eye-tracking prediction.
