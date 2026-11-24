# Beyond Explicit Toxicity

This repository contains a German–Greek corpus for research on explicit and implicit toxic language, developed within EmoBot, an LLM-based educational system for second and foreign language learning. Both language components contain written text and use the same three-layer annotation scheme for toxicity type, bias type, and target type.

The accompanying notebook documents the classifier training used to establish experimental baselines for the corpus. The resource can support research on content filtering, dialogue safety, and detoxification. The paper evaluates classification performance on the corpus.

> **Content warning:** The corpus contains offensive, abusive, and discriminatory language.

## Repository structure

.
├── data/                               # German and Greek data and experimental splits
├── guidelines/                         # Annotation guidelines
├── models/                             # Trained baseline models (to be added)
├── notebooks/
│   └── toxic_classifier_training.ipynb # Baseline training and experimentation
├── src/                                # Training, evaluation, and inference scripts (to be added)
├── results/                            # Evaluation outputs (to be added)
└── README.md


## Datasets

The corpus comprises German (DE) and Greek (EL) components. The German component contains selected records from five existing corpora that were manually re-annotated under the shared scheme. It comprises 210,518 tokens. The Greek component contains newly collected social media posts.

Four trained linguists contributed to the annotation. Inter-annotator agreement was assessed using Krippendorff’s alpha on independently annotated subsets of 150 records per language. Both components use adjudicated labels for toxicity type, bias type, and target type.

The table reports record counts for the experimental splits. The German row gives the original partitions.

| Language | Dev | Train | Test | Total |
| --- | ---: | ---: | ---: | ---: |
| German (DE) | 744 | 5,951 | 744 | 7,439 |
| Greek (EL) | 531 | 4.250 | 532 | 5,313 |
| **Total** | 1,275 | 10,201 | 1,276 | 12,752 |



## Team

- Voula Giouli, Aristotle University of Thessaloniki
- Stella Markantonatou, ATHENA RC
- Antonis Balas, Aristotle University of Thessaloniki
- Elina Zioga, Aristotle University of Thessaloniki
- Rodanna Konstantinidi, Aristotle University of Thessaloniki
- Elena Triantafyllidi, Aristotle University of Thessaloniki

## To cite this work

If you use the corpus, please cite *Beyond Explicit Toxicity: A German–Greek Dataset for Implicit Toxic Speech Detection*, accepted to Findings of EACL 2027.

<!-- Add the official citation and ACL Anthology link once available. -->

## Acknowledgments

This work was supported by Greece’s National Recovery and Resilience Plan (NRRP), “Greece 2.0,” through the “Clusters of Research Excellence” (CREs) program (SUB1.1), under the project “Interactive Agent with Emotional Intelligence for Second/Foreign Language Learning” (EmoBot, project code ΟΠΣ ΤΑ 5180519). This work also received partial funding from the Special Account for Research Funds (ELKE) of Aristotle University of Thessaloniki.
