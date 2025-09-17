# ParlaMint-SI Political Identity Analysis

The repository contains data analysis of the Slovenian parliamentary corpus ParlaMint-SI corpus, 
with a focus of exploring political identities in the parliamentary context. 
The analysis emphasises three main categories, that are one of the building blocks of political identity, that can be traced through metadata:

- *Membership*: formal, "card-carrying" affiliations such as membership in a political party/parliamentary group and institutional roles
- *Group relations*: dynamics and affiliations with different political groups (e.g. coalition and opposition)
- *Ideology*:  broader ideological positioning of parties

## Data
The analysis is based on the ParlaMint-SI corpus, a linguistically annotated dataset of parliamentary proceedings from Slovenia.
For analysis and demonstration purposes, a sample of the corpus is used here, which is stored in the folder [Sample](./Sample/) together with the
Chapel Hill Expert Survey dataset, which was filtered for Slovenian data only and matched with ParlaMint-SI party IDs.

## Repository structure
- [Notebooks](./Notebooks/): Jupyter notebooks with step-by-step analysis.
- [Sample](./Sample/): Sample data, available for analysis demonstration and reproduction.
- [Results](./Results/): Outputs of the (sample) analysis (figures, tables, reports)