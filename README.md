# Differentiable Gillespie Algorithm (DGA)

This repository contains the code and experimental data associated with the paper titled "A Differentiable Gillespie Algorithm for Simulating Chemical Kinetics, Parameter Estimation, and Designing Synthetic Biological Circuits" by Krishna Rijal and Pankaj Mehta [1].

## Repository Structure

- `jsd_analysis/`
  - `a_vs_jsd.ipynb`: Jensen-Shannon divergence (JSD) versus the hyper-parameter $a$.
  - `b_vs_jsd.ipynb`: JSD versus the hyper-parameter $b$. 
  - `sim_time_vs_jsd.ipynb`: JSD versus simulation time.

- `simulated_data_fitting/`
  - `random_rates.npy`: Data file with random rates for the two-state promoter model.
  - `2state_model_no_degeneracy.ipynb`: Learning the parameters $\left(k_{\text{on}}^{\text{R}}, r\right)$ of the two-state promoter model for the non-degenerate scenario.
  - `2state_model_no_degeneracy_error_bars_on_kon.ipynb`: Error bars on $k_{\text{on}}^{\text{R}}$ for the two-state promoter model for the non-degenerate scenario.
  - `2state_model_no_degeneracy_error_bars_on_r.ipynb`: Error bars on $r$ for the two-state promoter model for the non-degenerate scenario.
  - `2state_model_error_bars_on_mean_and_std.ipynb`: Error bars on the mean and standard deviation for the two-state promoter model.
  - `2state_model_with_degeneracy.ipynb`: Learning the parameters $\left(k_{\text{on}}^{\text{R}}, r, \gamma \right)$  of the two-state promoter model for the degenerate scenario.
  - `2state_model_loss_function_heat_maps_with_degeneracy.ipynb`: Heat maps of the loss function for the two-state promoter model for the degenerate scenario.

- `science_paper_exp_data_fitting/`
  - `science_data_5DL1.npy`: Experimental data for the 5DL1 promoter.
  - `science_data_lacUD5.npy`: Experimental data for the *lac*UD5 promoter.
  - `5DL1_data_fitting.ipynb`: Learning the parameters $\left(k_{\text{on}}^{\text{R}}, r, \gamma\right)$ of the two-state promoter model for the 5DL1 promoter data.
  - `5DL1_data_fitting_errors.ipynb`: Error analysis for the 5DL1 promoter data fitting.
  - `lacUD5_data_fitting.ipynb`: Learning the parameters $\left(k_{\text{on}}^{\text{R}}, r, \gamma \right)$ of the two-state promoter model for the *lac*UD5 promoter data.
  - `lacUD5_data_fitting_errors.ipynb`: Error analysis for the *lac*UD5 promoter data fitting.

- `loop_promoter_designing/`
  - `loop_model_response1.ipynb`: Learning the seven parameters of the loop promoter model for response-1.
  - `loop_model_response2.ipynb`: Learning the seven parameters of the loop promoter model for response-2.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- NumPy
- PyTorch
- Matplotlib
- SciPy

### Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/Emergent-Behaviors-in-Biology/Differentiable-Gillespie-Algorithm.git
    ```

2. Navigate to the project directory:
    ```bash
    cd DifferentiableGillespieAlgorithm
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

### Running the Notebooks

Open Jupyter Notebook:
```bash
jupyter notebook
```

Navigate to the notebook you want to run and execute the cells.

###  **Usage**

Each Jupyter notebook in this repository is self-contained. The notebooks are organized into different directories (jsd_analysis, loop_promoter_designing, science_paper_exp_data_fitting, simulated_data_fitting) based on their purpose. Appropriate functions are defined and described within the notebooks. The codes are well-commented to facilitate understanding and replication of the results.

## **Acknowledgements**

This work was supported by NIH NIGMS R35GM119461 and the Chan Zuckerberg Initiative Investigator grant to P.M. We also acknowledge support from the Shared Computing Cluster (SCC) administered by Boston University Research Computing Services.

## **Citation**

Rijal, K. and Mehta, P. (2025). A Differentiable Gillespie Algorithm for Simulating Chemical Kinetics, Parameter Estimation, and Designing Synthetic Biological Circuits. eLife, 14:RP103877. DOI: 10.7554/eLife.103877
