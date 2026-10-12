# Data Cleaning

A hands-on introduction to cleaning a real, messy dataset with pandas. Working through a raw Seattle weather file, you fix column names, remove duplicates, correct data types and units, standardize categorical labels, and handle missing values. Data cleaning is one part of an exploratory data analysis (EDA), so this notebook gives you a foundation for your first project.

## Learning Objectives

By the end of this repository, you should be able to:

- Inspect a raw dataset and identify common data quality issues.
- Standardize column names and remove duplicate rows.
- Fix data types and transform values: dates, units, and categorical labels.
- Handle missing data by dropping rows or imputing (constant, mean/median/mode, interpolation).
- Visualize missing values with missingno to look for patterns.

## Learning Path

| File / Folder | Description |
|---|---|
| [**01 - Data Cleaning**](01_data_cleaning.ipynb) | Clean a raw Seattle weather dataset end to end: inspect, fix column names, drop duplicates, correct data types and units, map categorical values, and impute missing data. |

### Additional Folders and Files

| File / Folder | Description |
|---|---|
| [**Data**](data/) | The raw `seattle-weather_raw.csv` dataset used in the notebook. |
| [**Solutions**](solutions/) | Reference solutions for the exercises. |
| [**pyproject.toml**](pyproject.toml) | Project configuration and dependencies. |
| [**uv.lock**](uv.lock) | Dependency lock file. |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a **placeholder**. Replace it, including the `< >` brackets, with your own value. For example, `cd <repo-name>` becomes `cd ds-data-cleaning`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> If you are working in pairs or groups, only **one person** should complete this step.

---

### 2. Add Collaborators (Pairs/Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

Teammates should accept the invitation before continuing.

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like `git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder and Install Dependencies

This installs all dependencies and creates a virtual environment in `.venv/`.

```bash
cd <repo-name>
uv sync
```

---

### 5. Open the Notebook

> [!NOTE]
> Make sure you open VS Code from the project root so it automatically detects the environment created by `uv sync`.

Launch VS Code in the project root folder:

```bash
code .
```

Then open `01_data_cleaning.ipynb` and select the Python environment created by `uv sync` as the kernel.

## References & Further Reading

- [**Pandas: Working with missing data**](https://pandas.pydata.org/docs/user_guide/missing_data.html): Official guide to detecting, dropping, and filling missing values.
- [**Pandas: Getting started tutorials**](https://pandas.pydata.org/docs/getting_started/intro_tutorials/index.html): Short, practical introductions to the core pandas workflow.
- [**Pythonic data cleaning with pandas and NumPy**](https://realpython.com/python-data-cleaning-numpy-pandas/): A worked tutorial that applies these same cleaning steps to other real datasets.
- [**Kaggle: Data Cleaning course**](https://www.kaggle.com/learn/data-cleaning): A short, free course with exercises on missing values, scaling, and inconsistent text entries.
