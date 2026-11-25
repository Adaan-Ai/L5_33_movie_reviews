# Lab 5 – Static Code Analysis: Movie Review System

## 1. Introduction

Static code analysis was performed on `movie_reviews.py` using three tools:

- Pylint – Code quality analysis.
- Bandit – Security vulnerability analysis.
- Flake8 – Python coding style analysis.

## 2. Issues Identified and Fixes

| Tool | Issue | Fix Applied |
|---|---|---|
| Pylint | Missing module docstring | Added module documentation |
| Pylint | Missing function docstrings | Added docstrings to functions |
| Pylint | Incorrect naming conventions | Converted function names to snake_case |
| Pylint | Unnecessary else statement | Removed unnecessary else |
| Pylint | Global statement usage | Removed unnecessary global variable |
| Pylint | Inefficient loop | Used enumerate() |
| Bandit | B104: Binding to all network interfaces | Changed 0.0.0.0 to 127.0.0.1 |
| Bandit | B105: Hardcoded password | Removed unused hardcoded password |
| Bandit | B311: Standard random generator | Used secrets.choice() |
| Bandit | B324: Weak MD5 hashing | Replaced MD5 with SHA-256 |
| Flake8 | E225: Missing whitespace around operator | Corrected spacing |
| Flake8 | E302: Incorrect blank lines | Added required blank lines |
| Flake8 | E261: Incorrect comment spacing | Corrected comment spacing |
| Flake8 | E231: Missing whitespace after comma | Corrected comma spacing |

## 3. Before and After Results

| Tool | Before | After |
|---|---|---|
| Pylint | 5.47/10 | 10.00/10 |
| Bandit | 4 issues | 0 issues |
| Flake8 | 4 violations | 0 violations |

## 4. Conclusion

Static code analysis helped identify code quality, security and formatting problems in the Movie Review System.

After implementing the necessary improvements, the program achieved a Pylint score of 10/10, with zero Bandit security findings and zero Flake8 violations.

The application continued to execute successfully after the modifications.
