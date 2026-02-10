# src

Project scripts for preprocessing, filtering, analysis, and visualization.

## Entry point
- `main.py` orchestrates the workflow by importing and calling the modules.

## Key scripts
- `data_preprocessing.py`: preprocessing utilities
- `zero.py`: zero-shot filtering of articles (soccer relevance)
- `script.py`: analysis helpers and statistics
- `visualization.py`: plots and figures
- `soccerNER_finetuner.py`: fine-tuning for token classification (soccer NER)
- `entity_extractor.py`: entity extraction using a local model folder

## Outputs
Do not commit:
- `DATA/` (input + intermediate data)
- `RESULTS/` (generated outputs)
