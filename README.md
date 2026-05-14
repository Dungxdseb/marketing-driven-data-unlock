# Marketing-Driven Data Unlock

This project focuses on analyzing and visualizing data of an ecommerce business to support decision-making in the marketing domain. The entire workflow — from data processing to report generation — is powered by tools like Jupyter Notebook and Python libraries.

## 🎯 Objectives

- Analyze  datasets to uncover valuable insights.
- Build BG/NBD model and apply to cluster sellers.
- Build visual reports and dashboards to present findings.
- Support data-driven decision-making.

## 🌳 Project Structure

```
.
├── .gitignore
├── .python-version
├── README.md
├── dashboard/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── EDA.ipynb
│   ├── K-mean.ipynb
│   ├── Stages.ipynb
│   ├── check_data_assumption.ipynb
│   ├── diagram.png
│   ├── metrics_and_plots.ipynb
│   └── top_k.ipynb
├── outputs/
├── pyproject.toml
├── report/
└── uv.lock
```

- `data/raw/`: Contains raw, unprocessed data.
- `data/processed/`: Contains cleaned and processed data ready for analysis.
- `notebooks/`: Contains Jupyter Notebook files for data analysis and exploratory data analysis (EDA).
- `dashboard/`: Contains source code for visual dashboards.
- `outputs/`: Stores output artifacts such as charts, CSV files, etc.
- `report/`: Contains compiled reports.
- `pyproject.toml`: Project configuration file and dependency declarations.
- `uv.lock`: Dependency lock file that ensures a consistent environment.

## 🛠️ Setup & Environment

This project uses `uv` to manage the Python environment and packages.

### 1. Prerequisites

- Install [Python 3.11](https://www.python.org/) or use `pyenv` to manage Python versions.
- Install `uv` (if not already installed). `uv` is an extremely fast Python package and environment manager.

  ```bash
  # macOS / Linux
  curl -LsSf https://astral.sh/uv/install.sh | sh

  # Windows (PowerShell)
  irm https://astral.sh/uv/install.ps1 | iex
  ```

### 2. Environment Setup

Run the following commands from the project root directory:

```bash
# 1. Create a virtual environment with uv
uv venv

# 2. Activate the virtual environment
# macOS / Linux
source .venv/bin/activate
# Windows
.venv\Scripts\activate

# 3. Install dependencies from the lock file
uv pip sync uv.lock
```

### 3. Register Jupyter Kernel

After activating the virtual environment, register it as a Jupyter kernel so notebooks always use the correct project environment:

```bash
# Install ipykernel into the virtual environment
uv pip install ipykernel

# Register the kernel with Jupyter
uv run python -m ipykernel install --user --name marketing-driven-data-unlock --display-name "Python (marketing-driven-data-unlock)"
```

> **Note:** The `--name` flag is a unique identifier (no spaces), while `--display-name` is what you'll see in the Jupyter kernel selector. You can verify registered kernels at any time with `jupyter kernelspec list`.

### 4. Run Jupyter Notebook

Once setup is complete, launch Jupyter Notebook or Jupyter Lab via `uv`:

```bash
# Run Jupyter Notebook
uv run jupyter notebook

# Or run Jupyter Lab
uv run jupyter lab
```

Your browser will automatically open the Jupyter interface. Navigate to the `notebooks/` directory to start working — and make sure to select the **"Python (marketing-driven-data-unlock)"** kernel from the kernel menu.

## 🤝 Contributing

Contributions are welcome! If you have ideas for improvements, new analyses, or code optimizations, feel free to open a Pull Request.

## 📄 License

Please contact us for licensing details.
Email: 1230523@st.neu.edu.com, 
       11230542@st.neu.edu.com, 
       11230543@st.neu.edu.com,
       11230560@st.neu.edu.com, 
       11230585@st.neu.edu.com
