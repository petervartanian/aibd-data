# Artificial Intelligence Benefits Database (AIBD)

Benefits of AI, each traced to its sources. This repository keeps every edition of the database that Peter H. Vartanian curates at [petervartanian.xyz/aibd](https://petervartanian.xyz/aibd/), one commit and one tag per edition, so that Software Heritage can archive each one in full. The site always shows the latest edition. Every edition is also on [Hugging Face](https://huggingface.co/datasets/petervartanian/AIBD). The database's DOI, the same for every edition, is [10.57967/hf/11470](https://doi.org/10.57967/hf/11470).

A benefit is one good from one system in one setting. A benefit reported in several sources is one benefit with several sources. A benefit that happened again elsewhere is an echo of the first.

## Files

The dataset is one file, `records.json`, with 1,148 benefits. Three flat tables come from it:

- `records.csv`, one row per benefit
- `ratings.csv`, one row for each rated kind of beneficiary
- `echoes.csv`, one row per attempt to make a benefit happen again

`schema.json` defines every field. `profiles.json` holds the public profile of each benefit, and `requirements.json` is the dictionary of its fields. `measurements.csv` and `measurements.json` give the measured outcomes. `collections.json` describes the collections, and each collection has its own JSON and CSV file. `manifest.json` gives the SHA-256 of every file in the edition.

Five files put the benefits under the questions of one document each, in that document's words:

- `for-procurement.csv`: OMB Memorandum M-25-22, section 4(b)(iii)
- `for-impact-assessment.csv`: OMB Memorandum M-25-21, section 4(b)(ii)
- `for-clinical-use.csv`: the Joint Commission and CHAI guidance on the responsible use of AI in healthcare, element 4
- `for-regulation.csv`: the AI Act, Article 7(2)(j)
- `for-court-use.csv`: UNESCO's Guidelines for the Use of AI Systems in Courts and Tribunals, principles 1.3, 1.6 and 1.13

`readers.json` gives each document's passage and address. A cell reads “not in the sources” when the sources were read for its question and do not answer it, and “not checked” when no one has read them for it yet.

## Evidence

A source supports a benefit only when its authors credit the AI system with at least part of it. The strongest support sets the grade:

- **Found.** A body with authority confirmed it.
- **Studied.** Independent researchers measured it.
- **Reported.** An independent outlet reported it from its own inquiries.
- **Claimed.** Only the parties to the benefit say so.

Each rated benefit also carries a certainty in GRADE's four levels, from very low to high. The [guide](https://petervartanian.xyz/aibd/guide.html) explains both.

## License and citation

The data are released under CC BY 4.0. The site has a [privacy notice](https://petervartanian.xyz/aibd/privacy.html).

```bibtex
@misc{vartanian_aibd,
  author = {Vartanian, Peter H.},
  title = {Artificial Intelligence Benefits Database},
  year = {2026},
  url = {https://petervartanian.xyz/aibd/},
  doi = {10.57967/hf/11470},
  note = {Edition 2026-11-06-442efa4d02b5}
}
```
