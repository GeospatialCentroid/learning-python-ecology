# learning-python-ecology
learning-python-ecology

# Conda Environment Setup: Jupyter, Pandas, & Plotnine

This guide walks through the complete setup for a clean Conda environment configured.
Conda is a package manager that allows you to install libraries that extend the core functionality available with python.



---

## 1. Instal Conda

To use Conda you'll first need to install [Conda Forge](https://conda-forge.org/download/). Choose the latest  version for your operating system from the web page, download and install

## 2. Create and Activate the Environment

Open your terminal or Anaconda Prompt and execute the following commands to set up the environment with Python 3.10:

```bash
# Create the environment
conda create -n learning_python

# Activate the environment
conda activate learning_python
```

---

## 3. Install Core Packages

Install Jupyter, `pandas`, `plotnine`, and `ipykernel` using the `conda-forge` channel for optimal package compatibility:

```bash
conda install -c conda-forge jupyter pandas plotnine ipykernel -y
```

---

## 4. Register the Environment as a Jupyter Kernel

To ensure this specific environment is visible and selectable inside the Jupyter Notebook interface, register it as a kernel:

```bash
python -m ipykernel install --user --name=learning_python --display-name "Learning Python"
```

---

## 5. Launch and Use

Launch your Jupyter interface:

```bash
jupyter notebook
```

### Switching to the Environment:
1. Open or create a notebook in your browser.
2. Navigate to the top menu and select **Kernel > Change Kernel**.
3. Choose **Python (data_viz)** from the dropdown list.

---

## Advanced Feature Installation

If your workflows require extended capabilities (such as integrating spatial data or advanced visualization options), you can install the extra dependencies for `plotnine` with this command:

```bash
conda install -c conda-forge "plotnine[extra]" -y
```
