# NLTK POS Tagging & Corpus Frequency Analysis

**A reproducible Python NLP laboratory exploring tokenization, grammatical tagging, morphological processing, and corpus statistics.**

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white) ![NLTK](https://img.shields.io/badge/NLTK-3.9.1-2F6B4F) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white) ![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00?logo=googlecolab&logoColor=white)

## Project Overview

This project demonstrates practical **Natural Language Processing (NLP)** using **Python and NLTK**, focusing on grammatical analysis and quantitative corpus exploration.

It includes sentence segmentation, word tokenization, stemming, lemmatization, part-of-speech tagging, and statistical analysis of the Brown Corpus and Penn Treebank.

Developed as an educational laboratory activity at **IIT Jodhpur**, the project emphasizes analytical reasoning, reproducible workflows, data validation, and technical documentation.

## Key Features

- Sentence segmentation and word tokenization using NLTK.
- POS tagging using default, rule-based, and pretrained statistical taggers.
- Porter Stemmer, Snowball Stemmer, and WordNet Lemmatizer comparison.
- POS frequency analysis using `FreqDist`.
- Brown Corpus analysis using native and Universal POS tagsets.
- Penn Treebank word-frequency and POS-frequency analysis.
- File reading, writing, appending, and last-line extraction.
- Corpus consistency checks and validation assertions.
- Analysis of lexical and structural ambiguity.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python 3 | Core programming |
| NLTK 3.9.1 | Natural Language Processing |
| Brown Corpus | Tagged corpus analysis |
| Penn Treebank | Word and grammatical tag analysis |
| WordNet | Lemmatization |
| FreqDist | Frequency computation |
| Jupyter Notebook | Interactive development |
| Google Colab | Cloud-based execution |
| Git and GitHub | Version control and documentation |

## System Workflow

```text
Input Text / Tagged Corpora
          |
          v
Sentence Segmentation
          |
          v
Word Tokenization
          |
          v
Stemming and Lemmatization
          |
          v
Part-of-Speech Tagging
          |
          v
Word and POS Frequency Analysis
          |
          v
Native vs Universal Tagset Comparison
          |
          v
Validation and Interpretation
```

## Recorded Results

The following measurements are taken from saved notebook execution outputs.

| Parameter | Result |
|---|---:|
| Brown Corpus Tokens | 1,161,192 |
| Brown Native POS Tags | 472 |
| Brown Universal POS Tags | 12 |
| Penn Treebank Tokens | 100,676 |
| Penn Treebank Unique Word Types | 12,408 |
| Penn Treebank Native POS Tags | 46 |
| Penn Treebank Universal POS Tags | 12 |
| Tagged Example Sentences | 6 |
| Morphological Comparison Words | 13 |
| Executed Code Cells | 20/20 |
| Saved Python Errors | 0 |
| Final Assertions | Passed in saved execution |

**Important:** These are recorded notebook results, not new independent benchmark measurements. POS frequency analysis does not measure model tagging accuracy.

## Installation and Setup

### Google Colab

1. Open Google Colab.
2. Upload `notebooks/AlokSahni-G25AIT2138-NLTK-POS-Tagging.ipynb`.
3. Select **Runtime → Run all**.
4. Allow the required NLTK resources to download.
5. Review exercise outputs and final validation.

### Local Environment

```bash
python -m venv .venv
python -m pip install -r requirements.txt
jupyter notebook
```

Activate the virtual environment before installation when working locally.

The notebook requires NLTK language resources including `punkt_tab`, `averaged_perceptron_tagger_eng`, `brown`, `treebank`, `wordnet`, and `universal_tagset`.

## Usage Example

```python
import nltk

nltk.download("punkt_tab")
nltk.download("averaged_perceptron_tagger_eng")

sentence = "A bright, colorful rainbow appeared today."

tokens = nltk.word_tokenize(sentence)
tagged = nltk.pos_tag(tokens)

print(tagged)
```

Examples of recorded POS assignments include:

- `bright` → `JJ` (Adjective)
- `appeared` → `VBD` (Past-tense Verb)
- `rainbow` → `NN` (Noun)

## Project Structure

```text
nltk-pos-tagging/
├── README.md
├── requirements.txt
├── notebooks/
│   └── AlokSahni-G25AIT2138-NLTK-POS-Tagging.ipynb
└── docs/
    └── PORTFOLIO_NEXT_STEPS.md
```

## Challenges and Solutions

| Challenge | Solution |
|---|---|
| NLTK resource availability | Included resource download setup |
| Different POS tag conventions | Compared native and Universal tagsets |
| Incorrect interpretation of tag frequency | Distinguished fine-grained and aggregate labels |
| Morphological variation | Compared stemming with WordNet lemmatization |
| Structural ambiguity | Documented POS tagging limitations |
| File reading without known length | Implemented streaming last-line extraction |
| Result consistency | Added assertion-based checks |

## Skills Demonstrated

- Python programming
- NLP text preprocessing
- POS tagging and grammatical analysis
- NLTK corpus processing
- Stemming and lemmatization
- Word-frequency analysis
- Corpus statistics and tagset mapping
- File handling
- Data validation
- Problem-solving and debugging
- Jupyter Notebook development
- Technical documentation

## Screenshots and Demo

Suggested screenshots to add after a fresh notebook run:

- Six-sentence POS tagging output.
- Brown Corpus native vs Universal POS distribution.
- Penn Treebank word-frequency analysis.
- Final validation assertions.

These are future additions and are not represented as existing images.

## Project Impact

- Completed a Python/NLTK workflow covering tokenization, stemming, lemmatization, and POS tagging.
- Analyzed recorded distributions over **1.16 million Brown Corpus tokens**.
- Compared Penn Treebank grammatical tag categories over **100,676 tokens**.
- Demonstrated native-to-Universal tagset conversion while preserving underlying corpus token counts.
- Implemented supporting consistency checks and documented linguistic ambiguity.

## Future Improvements

1. Refactor repeated notebook functions into reusable Python modules.
2. Add automated regression tests using `pytest`.
3. Integrate GitHub Actions for notebook-related checks.
4. Create frequency-distribution visualizations.
5. Evaluate POS tagging accuracy on held-out labeled data.
6. Explore dependency parsing and contextual word embeddings.
7. Add a transformer-based NLP classification project.

## Contributing

Educational contributions and improvements are welcome, subject to coursework-sharing policies.

Open an issue describing the problem, make changes on a feature branch, test the implementation, and submit a pull request.

Do not upload confidential data or third-party course material without permission.

## License

No open-source license is currently specified. Confirm ownership and redistribution permissions before adopting a license.

## Acknowledgments

Developed as part of the Natural Language Processing laboratory coursework at **IIT Jodhpur** using the NLTK library.

**Student:** Alok Sahni  
**Roll Number:** G25AIT2138

---

**Project scope:** Educational NLP processing and corpus-analysis workflow—not a deployed NLP service or newly trained language model.
