---
layout: page
title: Shared Task
permalink: /shared_task
---

## Shared Task: Cross-linguistic Prediction of Human Reading Behavior

The benefits of eye movement data for machine learning have been assessed in various domains, including NLP and computer vision. Eye tracking provides millisecond-accurate records on where humans look when they are reading and are useful in explanatory research of language processing. Eye movements depend on the stimulus and are therefore language-specific but there are universal tendencies which remain stable across languages (Liversedge et al., 2016). Modelling human reading has been researched extensively in psycholinguistics (e.g., Reichle et al., 1998; Matthies & Søgaard, 2013; Hahn & Keller, 2016; Sood et al., 2008). Being able to accurately predict eye-tracking features across languages will advance this field and will facilitate comparisons between models and the analysis of their varying capabilities.

### Task

In this shared task we address the challenge of predicting eye-tracking features recorded during sentence processing of multiple languages. We are interested in both cognitive modelling approaches as well as linguistically motivated approaches (i.e., language models). All teams are encouraged to write a short system description paper after the evaluation to present their models and results (see timeline below).

There are two major changes compared to the CMCL 2021 Shared Task on eye-tracking prediction:

    Multilingual data: We provide an eye movement dataset with sentences from six languages (Chinese, Dutch, English, German, Hindi, Russian).
    Eye-tracking features: To take into account the individual differences between readers, the task is not limited to predict the mean eye tracking features across readers, but also the standard deviation of the feature values.


### Task objective

The shared task if formulated as a regression task to predict 2 eye-tracking features and the corresponding standard deviation across readers:

    first fixation duration (FFD), the duration of the first fixation on the prevailing word;
    standard deviation of FFD across readers;
    total reading time (TRT), the sum of all fixation durations on the current word, including regressions;
    standard deviation of TRT across readers.

### Subtasks

    Subtask 1: Predict eye-tracking features for sentences of the 6 provided languages
    Subtask 2: Predict eye-tracking features for sentences from a new surprise language


## Links and Contacts

- For data and submission details, visit: [CODALAB, https://competitions.codalab.org/competitions/36415](https://competitions.codalab.org/competitions/36415)
- For questions, contact: [cmcl2021sharedtask@gmail.com](mailto:cmcl2021sharedtask@gmail.com)


Timeline

    December 6, 2021: Trial data release
    December 20, 2021: Participant registration opens & training data (& dev data) release
    January 10, 2023: Participant registration deadline
    January 19, 2022: Test data release
    February 1, 2022: Submission deadline for system predictions
    February 6, 2022: Results release
    February 28, 2022: Submission deadline for systems description papers
    March 26, 2022: Notification of Acceptance
    April 10, 2022: Camera-ready papers due
    May 26-28, 2022: CMCL Workshop (@ACL)


### Data

We will use the eye-tracking data recorded during natural reading from 8 datasets in 6 languages (see "Data" for details). The training data contains 1703 sentences, the development set contains 104 sentences, and the test set 324 sentences. The data provided will contain scaled features in the range between 0 and 100 to facilitate evaluation via the mean absolute average (MAE). The eye-tracking feature values are averaged over all readers.


## Evaluation

We will evaluate the prediction against the ground truth using the mean absolute error (MAE).
The winning system will be the one with the best average MAE across all 5 eye-tracking features.


## Papers

System description papers will be short papers (4 pages + references) describing the approach used for the eye-tracking prediction.
