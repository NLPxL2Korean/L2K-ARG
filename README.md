# Corpus Description

## Overview

This repository provides an open-access corpus of argumentative essays written by learners of Korean as a second language (L2 Korean). The dataset includes:

* Raw learner essays (raw_txt)
* Morphosyntactic annotations in CoNLL-U format (conllu)
* Learner proficiency information (metadata)

---

# Participants and Prompt Design

 The corpus contains 484 argumentative essays produced by learners from diverse L1 backgrounds (Last updated: May 2026):

| L1 Group | Description      | # of Essays |
| -------- | ---------------- | ---------------: |
| CHN      | Chinese          |               72 |
| CZH      | Czech            |              120 |
| ENG      | English          |              117 |
| HENG     | Heritage English |               49 |
| JPN      | Japanese         |              126 |


Due to differences in data collection settings, the prompts varied slightly across groups.

The CHN group responded to two prompts:

| Number | Prompt                                                                                 |
| ------ | -------------------------------------------------------------------------------------- |
| 1      | Which do you think is more important: conservation of nature or development of nature? |
| 2      | Which do you prefer: competition or cooperation?                                       |

The remaining groups (CZH, ENG, HENG, and JPN) responded to three prompts:

| Number | Prompt                                              |
| ------ | --------------------------------------------------- |
| 1      | Is early language education necessary for children? |
| 2      | Do we need to learn history?                        |
| 3      | Which do you prefer: competition or cooperation?    |

---

# Proficiency Measures

## General Korean Proficiency

All participants completed a Korean C-test designed to measure overall Korean language proficiency. The resulting C-test scores are included in the metadata file for all learner groups.

## Writing Proficiency Scores

In addition to the C-test, writing proficiency ratings were collected for the three learner groups that responded to the same set of prompts:

* CZH
* ENG
* JPN

---

# Corpus Structure

```text
L2K-ARG/
├── raw_txt/
│   ├── ARG-CHN_1_1.txt
│   ├── ARG-CHN_1_2.txt
│   └── ...
│
├── conllu/
│   ├── ARG-CHN_1_1.conllu
│   ├── ARG-CHN_1_2.conllu
│   └── ...
├── corpus.jsonl
├── metadata_c-test.csv
├── metadata_writing_scores.csv
└── writing_scoring_rubric.pdf
```

---

# File Naming Convention

Essay filenames follow the format:

```text
ARG-[GROUP]_[PARTICIPANT_ID]_[TOPIC_ID]
```

Example:

```text
ARG-CHN_1_2
```

where:

* `CHN` = learner group
* `1` = participant ID
* `2` = topic number

---

# License and Citation

- This project is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.
- For detailed information about the corpus, please see the following paper. 
  * Sung, H., Shin, G.-H., Jung, B.-K., & Jeong, E.-S. (2026). [L2K-ARG: Introducing and evaluating a learner corpus of Korean argumentative writing](https://doi.org/10.1075/ijlcr.26007.sun). *International Journal of Learner Corpus Research*. [[Preprint](https://www.researchgate.net/publication/411036996_L2K-ARG_Introducing_and_evaluating_a_learner_corpus_of_Korean_argumentative_writing)]
  * If you use the corpus in your research, we would greatly appreciate it if you could cite the paper above.

