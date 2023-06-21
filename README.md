## 1 Purpose of this repo
This repository serves as an introduction to [pre-commit](https://pre-commit.com/), a powerful tool designed to enhance code quality and enforce consistent coding standards. It showcases a range of impressive checks and formatting features that can significantly improve the overall quality and consistency of your codebase.

To achieve this, the repository leverages three key tools:

- [Black](https://pypi.org/project/black/): A highly regarded code formatter that automatically formats code to adhere to a consistent style guide, known as "black formatting." By applying opinionated rules, Black helps ensure that code has a consistent layout, making it easier to read and maintain. 

- [Ruff](https://pypi.org/project/ruff/0.0.89/): A comprehensive static code analysis tool that identifies potential issues (such as syntax errors, programming mistakes, style violations, and so on) and provides valuable suggestions for improving code quality.

- [Mypy](https://mypy.readthedocs.io/en/stable/): A powerful static type checker for Python that helps catch type-related bugs and provides increased clarity and reliability to your code.

By combining these tools with pre-commit, you can seamlessly integrate them into your development workflow. This enables automatic code formatting, thorough static analysis, and type checking, ensuring that your codebase meets the highest standards of quality and maintainability.


</br>

## 2 Setting it up

To use `pre-commit`in your projects, don't forget to configure the [pre-commit config file](.pre-commit-config.yaml) and the [pyproject.toml](pyproject.toml). 

The `pyproject.toml` file is used as a configuration file that specifies various settings and dependencies for the project (metadata, build configurations, and tool settings). 

</br>

## 3 Running locally
To run locally, you will need Python 3.11 or newer installed in your local environment. Then, just install the dependencies and execute the `main.py` file:

Create a virtual environment:
```
python3 -m venv .venv
```

Activate local environment:
```
source .venv/bin/activate
```

Install dependencies:
```
pip install -r requirements.txt
```

Install git hooks
```
pre-commit install
```

Now you can try to run script to see if everything is correctly set up so far (optional):
```
python3 src/main.py
```

Or just commit to see pre-commit in action!