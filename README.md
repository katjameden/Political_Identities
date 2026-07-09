# Analysis of political identity markers in Slovenian parliamentary debates

This repository contains the analyses of the Slovenian parliamentary corpus ParlaMint-SI, focusing on the exploration of markers of political identity.

The framework for this study encomapsses three individual analyses of markers of political identity-building categories in Slovenian parliamentary debates, which includes a [metadata-focused approach](./Metadata_Analysis/) to facilitate the discovery of various trends in parliamentary activity during the period covered by the corpus (2000–2022), as well as [concordancer-assisted discourse analysis](./Discourse_Analysis/) that enables the investigation of expressions of political identities through the concept of Us vs. Them, or more specifically, the pronouns "vaši" ("your") and "naši" ("our"). Lastly, the co-occurences of the terms "vaši" and "naši" are [explored in web and social media corpora](./Cross-corpus_Analysis/).

The results of the analyses are described in the following publications: 
```
@inproceedings{meden2026ours,
  title={Ours and Yours: A Discourse Analysis of Political Identity Markers in Slovenian Parliamentary Discourse},
  author={Meden, Katja},
  booktitle={Proceedings of the ParlaCLARIN V Workshop on Interoperability, Multilinguality, and Multimodality in Parliamentary Corpora @ LREC 2026},
  pages={13-21},
  year={2026}
}

@inproceedings{meden2026metadata,
    author = {Meden, Katja and Erjavec, Tomaž},
    title = {{Tracing Political Identities Through Metadata in Slovenian Parliamentary Debates}},
    note = {In print},
    booktitle = {Proceedings of the CLARIN Annual Conference 2026},
    year = {2026},
}

```

## Data
The analysis is based on the ParlaMint-SI 5.1.ana corpus, a linguistically annotated dataset of parliamentary proceedings of Slovenian Parliament (Državni zbor), which is currently available only in beta form, to be made available in the next official ParlaMint release. Replication with [ParlaMint-SI.ana 5.0](http://hdl.handle.net/11356/2005) yields minor frequency differences but does not affect the overall conclusions.
The corpus also incorporates data from the Chapel Hill Expert Survey dataset, which was filtered for Slovenian data only and matched with ParlaMint-SI party IDs.


## Metadata analysis
- [Sample](./Sample/): Sample data, available to run the metadata analysis (for demonstration purposes). 
- [Notebooks](./Notebooks/): Jupyter notebooks with step-by-step analysis (analysis outputs are based on the full dataset, but can be used to run the sample for demonstration purposes).
- [Results](./Results/): Outputs of the (sample) analysis (figures, tables, reports, included in Chapter III of the Thesis)

## Discourse analysis
The discourse analysis was conducted using the [NoSketch Engine](https://www.clarin.si/ske/#open) concordancer for the ParlaMint-SI 5.1 version of the corpus. The folder includes: 
- [Collocation Analysis](./Discourse_Analysis/Collocation_Analysis/): Analysis of the L0R1 collocations of all subcorpora and their results in TSV file format.
- [Keyword Analysis](./Discourse_Analysis/Keyword_Analysis/): Analysis of the representative keywords for each subcorpus and the concordancer outputs in TSV file format.

## Context analysis

- [Cross corpus analysis](./Cross-corpus_Analysis/): Outputs of the comparison of "naš" and "vaš" terms within different (parliamentary, web and social media) corpora and the results of the analysis (TSV). 
The repository also includes two Markdown files ([Discourse_Analysis](./Discourse_Analysis/Discourse_Analysis.md), [Cross-corpus comparison](./Discourse_Analysis/Cross-corpus%20comparison.md)), which includes the notes and detailed documentation of the discourse and cross-corpus analysis setup and results, as well as documentation of initial experiments, which helped in setting the parameters for the analysis.
