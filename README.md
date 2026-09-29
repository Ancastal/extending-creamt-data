# Extending CREAMT data

Research data for *Extending CREAMT: Leveraging Large Language Models for Literary Translation Post-Editing* (Castaldo et al., 2025).

The release contains an English-to-Italian literary translation study with a 141-line source and reference text: machine-translation outputs, final post-edited translations, and comparative annotation exports.

## Data

| Path | Contents |
| --- | --- |
| [`data/inputs/`](data/inputs/) | English source and published Italian reference translation |
| [`data/machine_translation/`](data/machine_translation/) | GPT-3.5, GPT-4, and Mistral outputs |
| [`data/final_translations/`](data/final_translations/) | Final translation conditions after controlled rotation |
| [`data/annotations/comparative/`](data/annotations/comparative/) | Comparative WebAnno/UIMA XMI annotation exports, organised by final condition |
| [`data/manifest.csv`](data/manifest.csv) | Condition-level inventory and paths |

Text files are UTF-8 plain text. The source and reference each have 141 lines; generated and final conditions retain their original segmentation and therefore contain 139–141 lines. Do not assume line-number alignment across conditions. XMI files retain their original export names and annotations.

## Method

Four professional translators worked in a controlled rotation: each translated one part of the original text from scratch and post-edited a different part for each machine-translation condition. Each final `from_*` file is therefore a composite of the four translators' work, not the work of one translator. See the paper for the full design and analysis.

## Citation

If you use these data, cite the accompanying paper. A ready-to-copy record is in [`paper.bib`](paper.bib); machine-readable metadata are in [`CITATION.cff`](CITATION.cff).

> Antonio Castaldo, Sheila Castilho, Joss Moorkens, and Johanna Monti. 2025. *Extending CREAMT: Leveraging Large Language Models for Literary Translation Post-Editing.* In *Proceedings of Machine Translation Summit XX: Volume 1*, pages 506–515, Geneva, Switzerland. European Association for Machine Translation.

Paper: <https://aclanthology.org/2025.mtsummit-1.40/>

## Rights and license

The research-created selection, organisation, machine outputs, post-edited outputs, and annotations are available under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). Attribution must include the citation above. See [`LICENSE`](LICENSE) and [`RIGHTS.md`](RIGHTS.md).

`data/inputs/source-en.txt` and `data/inputs/reference-it.txt` reproduce an excerpt and a published Italian reference translation of a copyrighted novel. They remain the property of their respective rightsholders and are supplied only for non-commercial scholarly research and reproducibility. This repository does not grant a licence to reuse them beyond rights held by the user or an applicable legal exception.
