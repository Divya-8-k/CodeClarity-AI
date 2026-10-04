# CodeClarity AI

CodeClarity AI is a beginner-friendly Python project that demonstrates prompt design for:

1. Bug explanation
2. Code-improvement suggestions

The project was developed and tested in Google Colab.

## Objective

The project designs prompts that help an AI/code-review system:
- Identify programming bugs
- Explain why a bug occurs
- Classify the error
- Suggest a fix
- Provide corrected code
- Review readability and structure
- Suggest efficiency, error-handling, security, and best-practice improvements

## Repository Structure

```text
CodeClarity-AI/
├── CodeClarity_AI.ipynb
├── sample_code.py
├── requirements.txt
├── README.md
└── .gitignore
```

## Example Input

```python
def calculate_average(numbers):
    total = sum(numbers)
    return total / len(numbers)

numbers = []
print(calculate_average(numbers))
```

## Detected Bug

The program attempts to divide by zero because the list is empty.

**Error Type:** Runtime Error

## Corrected Code

```python
def calculate_average(numbers):
    if not numbers:
        return 0
    return sum(numbers) / len(numbers)

numbers = []
print(calculate_average(numbers))
```

## Prompt Design

### Bug Explanation Prompt

The prompt asks the system to:
- Identify the problem
- Explain why it occurs
- Classify the error
- Explain how to fix it
- Provide corrected code

### Code Improvement Prompt

The prompt asks the system to review:
- Readability
- Structure
- Efficiency
- Error handling
- Security
- Best coding practices

## Running the Project

1. Open `CodeClarity_AI.ipynb` in Google Colab.
2. Run the notebook cells from top to bottom.
3. Review the generated prompts and final analysis.

## Technologies

- Python
- Google Colab
- Prompt Engineering
- Basic Code Analysis
- Hugging Face Transformers (optional/experimental)

## Author

Dharshini A.
