# NLP Exam Project — Football Article Analysis (ACL-style)

**One-liner:** Football-related news/articles → zero-shot filtering + entity extraction + analysis/visualization → produce filtered datasets and plots.

## Why it matters
A practical NLP workflow often starts with noisy text and needs robust filtering before analysis.
This project demonstrates an end-to-end approach: classify relevance, extract entities, and visualize patterns.

## Data
This repo expects local data folders under `src/` (not committed to git):
- `src/DATA/`: input datasets and intermediate files
- `src/RESULTS/`: generated outputs (tables, plots, artifacts)

Constraints:
- Large datasets and generated outputs should not be tracked in git.
- Some scripts assume specific local file paths/structures inside `src/DATA/`.

## Method
- `src/data_preprocessing.py`: preprocessing utilities
- `src/zero.py`: zero-shot filtering of articles (soccer vs non-soccer)
- `src/script.py`: dataset analysis and label distribution calculations
- `src/visualization.py`: plotting/visualization utilities
- `src/soccerNER_finetuner.py`: fine-tuning code for token classification (soccer NER)
- `src/entity_extractor.py`: entity extraction pipeline using a local model folder
- `src/main.py`: entry script that ties modules together

## Results
Status: Code and report are included. Outputs are generated locally into `src/RESULTS/`.

Included document:
- `NLP_Exam_Project_ACL__Marcel__Damian_.pdf`

## Repo structure
```text
nlp-exam-project/
├─ README.md
├─ requirements.txt
├─ .gitignore
├─ NLP_Exam_Project_ACL__Marcel__Damian_.pdf
└─ src/
   ├─ README.md
   ├─ main.py
   ├─ data_preprocessing.py
   ├─ zero.py
   ├─ script.py
   ├─ visualization.py
   ├─ entity_extractor.py
   ├─ soccerNER_finetuner.py
   ├─ GLiNER-json.py
   └─ zero on first 2 results.py
