# ParlaMint-SI Political Identity Analysis

This repository contains data analysis of the Slovenian parliamentary corpus ParlaMint-SI, focusing on the exploration of expressions of political identities in the parliamentary context.

The analysis includes a [metadata-focused approach](./Metadata_Analysis/) to facilitate the discovery of various trends in parliamentary activity during the period covered by the corpus (2000–2022), as well as [concordancer-assisted discourse analysis](./Discourse_Analysis/) that enables the investigation of expressions of political identities through the concept of Us vs. Them, or more specifically, the pronouns "vaši" ("your") and "naši" ("our").
## Data
The analysis is based on the ParlaMint-SI corpus, a linguistically annotated dataset of parliamentary proceedings from Slovenia. It also incorporates data from the Chapel Hill Expert Survey dataset, which was filtered for Slovenian data only and matched with ParlaMint-SI party IDs.
## Metadata Analysis
- [Sample](./Sample/): Sample data, available to run the metadata analysis (for demonstration purposes). 
- [Notebooks](./Notebooks/): Jupyter notebooks with step-by-step analysis (analysis outputs are based on the full dataset, but can be used to run the sample for demonstration purposes).
- [Results](./Results/): Outputs of the (sample) analysis (figures, tables, reports, included in Chapter III of the Thesis)

## Discourse Analysis
The discourse analysis was conducted using the [NoSketch Engine](https://www.clarin.si/ske/#open) concordancer for the ParlaMint-SI 5.1 version of the corpus. The folder includes: 
- [Collocation Analysis](./Discourse_Analysis/Collocation_Analysis/): Analysis of the L0R1 collocations of all subcorpora and their results in TSV file format.
- [Keyword Analysis](./Discourse_Analysis/Keyword_Analysis/): Analysis of the representative keywords for each subcorpus and the concordancer outputs in TSV file format.
- Cross corpus analysis: Outputs of the comparison of "naš" and "vaš" within different (parliamentary, web and social media) corpora and the results of the analysis (TSV). 
The repository also includes two Markdown files ([Discourse_Analysis](./Discourse_Analysis/Discourse_Analysis.md), [Cross-corpus comparison](./Discourse_Analysis/Cross-corpus%20comparison.md)), which includes the notes and detailed documentation of the discourse and cross-corpus analysis setup and results.