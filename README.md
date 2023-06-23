# Protein-protein interaction

Notebook to fit the model described in [Roehrl *et al*, Biochemistry 43.51 (2004): 16056-16066](https://pubs.acs.org/doi/full/10.1021/bi048233g?casa_token=rlvgtYAYetcAAAAA%3Av59DOeTp14qDL3OZDasWt-_LJYpS1buuMrQI9McanroG3nbRCansk8UERtaN8XlYoF2zyAInV6gE2Fqx) to experimental data.


## Installation

We use conda to set up a specific Python environment containing all the packages we want to use.

1. Download this repository (either by using `git clone https://github.com/nobias-fht/competitive_binding.git` on the terminal or just downloading and unzipping).
2. If you don't have `conda`, install [miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html)
3. In the command line terminal, navigate to the repository and type `conda env create -f env.yml`
4. Activate environment: `conda activate protprot`
5. Finally, start jupyter notebook by typing `jupyter notebook` and use the notebook.


## Data format

The notebook expects the following format. for the `.csv` file:


| L_T (uM) | C1 replicate 1 (%) | ... | C2 replicate 1 (%) | ... |
|----------|:------------------:|:---:|:------------------:|:---:|
| 0.01     | 56.23              | ... | ...                | ... |
| 0.1      | ...                | ... | ...                | ... |
| 10       | ...                | ... | ...                | ... |


The values should be separated by a comma (`,`) and the decimals indicated by a dot (`.`). Check out [the example file](example.csv).

:warning: Make sure your data is in the proper format!
