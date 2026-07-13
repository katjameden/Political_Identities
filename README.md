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

## Repository data and methods

This repository contains the code, data, and outputs for a mixed-method analysis of parliamentary identity construction, combining metadata analysis of parliamentary structures with corpus-assisted discourse analysis of parliamentary speeches.
The analyses are based on the ParlaMint-SI 5.1.ana corpus, a linguistically annotated dataset of parliamentary proceedings of Slovenian Parliament (Državni zbor), which is currently available only in beta form, to be made available in the next official ParlaMint release. Replication with [ParlaMint-SI.ana 5.0](http://hdl.handle.net/11356/2005) yields minor frequency differences but does not affect the overall conclusions.
The corpus also incorporates data from the [Chapel Hill Expert Survey dataset](https://www.chesdata.eu/ches-europe) (using the 1999-2019 trend file, [Jolly et al.](https://doi.org/10.1016/j.electstud.2021.102420)), which was filtered for Slovenian data only and matched with ParlaMint-SI party IDs.

## Metadata analysis
[Metadata analysis](./Metadata_Analysis/) provides an overview of trends across the legislative period represented in the corpus (2000–2022, from the 3rd to the 8th legislative period). The metadata analysis examines four categories of political identity (PI) building proposed by van Dijk (2010): **Membership**, **Ideology**, **Group relations**, and **Power resources**. Within this study, the categories primarily relate to the following parliamentary structures:

- **Membership**: Political parties, and by extension parliamentary groups, constitute the primary unit of analysis. This category captures the composition and organisation of parliamentary actors.

- **Group relations**: This category primarily concerns the coalition and opposition status of parties, as well as the relationships between them.

- **Ideology**: Although a distinction should be made between ideology and political orientation, the two overlap to some extent. Party positions are captured using three CHES variables: the general left–right dimension (`lrgen`), the economic left–right dimension (`lrecon`), and the cultural dimension (`galtan`). Together, these measures situate parties within the broader ideological landscape.

- **Power resources**: This category is examined through key parliamentary processes, including changes across legislative periods and shifts in government structures.

Other PI-building categories proposed by van Dijk (2010)—**Activities/Discourse**, **Aims**, and **Norms & Values**—are more directly expressed through parliamentary speech and are therefore examined primarily through discourse analysis.

## Discourse analysis
[Discourse analysis](./Discourse_Analysis/) focuses on parliamentary speech and examines identity markers through a corpus-assisted approach. It combines text-type analysis, collocation analysis, and keyword analysis to investigate patterns of identity construction in parliamentary discourse.
The analysis draws on the concept of **Us versus Them** and examines how collective identities are constructed through the use of possessive pronouns, particularly *naš* ("our") and *vaš* ("your").

The analysis was conducted using the [NoSketch Engine](https://www.clarin.si/ske/#open) concordancer for the ParlaMint-SI 5.1 version of the corpus. 


## Context analysis
[Cross-corpus analysis](./Cross-corpus_Analysis/) examines the co-occurrence of *naši*...*vaši* (“"ours...yours"), a common linguistic pattern used to express political division in Slovenian discourse. The findings are then compared with patterns observed in web and social media discourse, which provide a broader perspective on the use of this dichotomy and its possible derivatives.

