# Digital Garden Helper

A CLI tool to tend your digital clutter like a garden ecosystem. Files grow from `seedling` → `blooming` → `overgrown` based on activity, and you get gentle suggestions to "prune" or "water" them.

## Features
- **Growth Stages**: Tag files/directories with visual indicators.
- **Ecosystem Feedback**: Directory-level health scores and summaries.
- **Low-Pressure Actions**: Suggestions to archive or review files.

## Usage
```bash
# Check the garden status
python src/main.py status

# Tend to a specific directory
python src/main.py tend /path/to/directory

# Prune (archive) a file/directory
python src/main.py prune /path/to/file_or_directory
```

## Installation
```bash
pip install -e .
```

