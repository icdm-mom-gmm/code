# Experiments
This repository contains code to reproduce the (synthetic) experiments from the paper 'Mixed Membership Gaussians on Siamese Representations' as submitted to ICDM 2021.

## Requirements
The following setup was tested on a Ubuntu 18.04.5 LTS system with CUDA Version: 10.2:

```
conda create --name icdmmom python=3.8 && conda activate icdmmom
pip install -r requirements.txt
```

## Defining Experiment
In order to define parameters for the experiment, change the parameter dictionary in *experiment.py*.
By default, the values are set to the values used in the paper.
## Starting Experiment
```
python experiment.py
```
## Results
Intermediate results will be saved as pickeled dictionaries (file `results/results_dict.p`), where keys are tracked quantities and values are lists of values.
The final result will be saved as pickeled pandas dataframe (file `results/final_result.p`). 
The results reported in the paper are saved as `results/original_result.p`.

To display the results from the paper and your own results, use
```
python load_results.py
```
