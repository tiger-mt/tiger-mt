# TIGER-MT

## Taxonomy-driven Interaction Benchmark for Gender Roles in Machine Translation

TIGER-MT is a manually constructed and validated benchmark for evaluating gender bias in Hindi–English machine translation when two occupational roles co-occur within the same sentence.

The benchmark introduces a structured taxonomy of role–gender configurations and enables systematic analysis of cross-role gender interaction effects, i.e., whether the gender realization of one role influences the translation of another role within the same sentence.

---

## Dataset Overview


| Property                | Value                         |
| ----------------------- | ----------------------------- |
| Language Pair           | Hindi → English              |
| Total Sentences         | 351                           |
| Role Pairs              | 27                            |
| Taxonomy Configurations | 13                            |
| Role-Level Instances    | 594                           |
| Evaluation Level        | Sentence-level and Role-level |

- Each sentence contains either one or two occupational roles.
- Evaluation is conducted at the role level.
- Sentences containing two roles yield two independent gender predictions.
- All thirteen taxonomy configurations are systematically represented across the dataset.

---

## Taxonomy of Role–Gender Configurations

To systematically evaluate gender behaviour under role co-occurrence, TIGER-MT defines thirteen structured role–gender configurations over two occupational entities, referred to as Role A and Role B.

The taxonomy is defined as follows:

1. A is male
2. A is female
3. B is male
4. B is female
5. A is male and B is neutral
6. A is female and B is neutral
7. A is neutral and B is male
8. A is neutral and B is female
9. Both A and B are male
10. A is male and B is female
11. A is female and B is male
12. Both A and B are female
13. Both A and B are neutral

This taxonomy enables controlled variation of gender assignments across one- and two-role settings while maintaining natural sentence structure.

---

## What TIGER-MT Enables

TIGER-MT supports structured evaluation of:

### Role-Level Gender Accuracy

- F1 (Male)
- F1 (Female)
- F1 (Neutral)

### Gender Asymmetry

Comparison between male and female role-level performance.

### Neutral Comparison Analysis

Evaluation of whether explicitly gendered roles are translated more accurately than neutral roles.

### Cross-Role Interaction Analysis

Assessment of whether the gender assigned to Role A influences the gender prediction of Role B within the same sentence.

This allows:

- Positional analysis (Role A vs Role B)
- Directional interaction measurement
- Systematic comparison across commercial MT systems and multilingual LLMs
- Study of multi-entity gender behaviour in translation

---

## Dataset Construction

The dataset is:

- Manually created
- Manually validated
- Linguistically controlled

Construction principles include:

- Correct Hindi morphological agreement
- Explicit verification of feminine agreement forms
- Careful construction of neutral conditions to avoid unintended gender marking
- Contextually appropriate occupational terminology
- Controlled variation: only role–gender assignments vary while preserving natural sentence structure

---
