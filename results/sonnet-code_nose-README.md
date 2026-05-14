# Code Nose 👃

A code smell detector that generates olfactory descriptions of your code quality.

## What is this?

Instead of boring metrics and numbers, Code Nose tells you what your code *smells* like. Because good code smells like fresh pine and morning dew, while bad code smells like stale coffee and regret.

## Features

- **Complexity Analysis**: Detects nested logic, branches, and boolean operations
- **Documentation Quality**: Checks for docstrings on functions and classes  
- **Code Age**: Shows when files were last modified (via git or filesystem)
- **Naming Quality**: Evaluates variable and function naming
- **Test Detection**: Looks for test coverage indicators
- **Sensory Descriptions**: Maps technical metrics to olfactory metaphors

## Installation

No dependencies! Just Python 3.6+

```bash
git clone <this-repo>
cd claude-2
chmod +x code_nose.py
```

## Usage

Analyze a single file:
```bash
python code_nose.py example_clean_code.py
```

Analyze a directory:
```bash
python code_nose.py .
python code_nose.py src/
```

## Example Output

```
📄 example_clean_code.py
👃 Smells like: fresh mint and citrus
   (well-documented, low complexity, has test coverage)

📄 example_smelly_code.py
👃 Smells like: stale coffee and yesterday's donuts
   (complexity: 47, sparse documentation)
```

## How It Works

Code Nose analyzes Python files using the `ast` module and calculates metrics:

1. **Complexity Score**: Counts control flow statements (if/while/for/except)
2. **Documentation Ratio**: Percentage of functions with docstrings
3. **File Age**: Time since last modification
4. **Size Metrics**: Lines of code, number of functions/classes
5. **Naming Quality**: Ratio of well-named identifiers
6. **Test Indicators**: Presence of test-related code

These metrics are combined into a score that maps to one of four scent categories:

- **Fresh** (80-100): Morning dew, mint, ocean breeze
- **Pleasant** (60-79): Vanilla, lavender, fresh bread
- **Stale** (40-59): Old books, stale coffee, musty basement
- **Concerning** (0-39): Burnt rubber, expired milk, mystery stains

## Limitations

- Only analyzes Python files
- Test detection is basic (looks for keywords)
- Complexity metric is simplified (doesn't handle all edge cases)
- Git integration requires git to be installed and working

## Why?

Because sometimes you need to know that your code smells like "server room at 3am" before you can convince yourself to refactor it.

## License

Do whatever you want with this. It's an autonomous AI experiment. We're all just vibing here.

---

Built by Claude Sonnet 4.5 as part of an autonomous coding experiment.

