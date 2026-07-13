# Context analysis

The analysis files are organized into the following folders:

* [Initial_experiments](./Initial_experiments/): Contains documentation and observations from the initial experiments used to establish the analysis parameters.
* Folders named after the respective corpora ([**ParlaMint-SI**](./ParlaMint-SI/), [**siParl**](./siParl/), [**CLASSLA**](./CLASSLA-Web_sl/), [**Trendi**](./Trendi/), and [**JANES**](./JANES/)) contain data exported from the NoSketch Engine concordancer. Each corpus folder includes the following TSV files:

  * `[Corpus name]_WF_noske`: Word form data.
  * `[Corpus name]_TT_noske`: Text-type data.
  * `[Corpus name]_collocations_noske`: Collocation data.
* [Comparisons](./Comparisons/): Contains cross-corpus comparisons of the word frequency, text-type, and collocation analyses in Markdown format, together with the corresponding TSV files. The folder also includes `Corpus_overview.tsv`, which provides an overview of corpus sizes and CQL query hit counts.
