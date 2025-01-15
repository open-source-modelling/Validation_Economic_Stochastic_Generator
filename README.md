# Economic Stochastic Generator Validation
Welcome to the Economic Stochastic Generator Validation project. This repository hosts three Jupyter notebooks which, contain a series of tests used to validate the correctness of outputs from an economic stochastic generator. The goal of this project is to provide a transparent, reproducible workflow for verifying generated economic scenarios and ensuring they align with expected statistical and economic properties.
________________________________________
## Overview
In many financial and economic applications, stochastic generators produce large volumes of scenarios to estimate future market behaviour. However, verifying that these scenarios are correct can be challenging. This project aims to give an open-source implementation that offers a structured approach to validating stochastic generator outputs against a set of known statistical and economic criteria.

Key Features:

- Three structured Jupyter notebooks for step-by-step validation.
- Clear documentation of each validation step (from data loading to result reporting).
- Using only basic Python and some commonly used Python packages.
- Easily extensible framework to suit different financial/economic models.
- Each notebook comes with some dummy data to serve as a starting point.
________________________________________
## Getting Started
### Prerequisites
- Python 3.8+
- Jupyter Lab or Jupyter Notebook
- Familiarity with Python data-analysis libraries (e.g., NumPy, Pandas, Matplotlib, SciPy)
### Data Preparation
1.	Download the entire repo
2.	Ensure that the test data is in the same folder as the notebook
3.	Open the Jupyter notebook for example in an Anaconda environment 
4.	Run the notebook
________________________________________
## Content:
#### Notebook 1: Validation of deterministic curves of a risk-neutral output
Purpose:
- Verify if the deterministic curves come from the same source as the regulator-released curves, and check if the curves are internally consistent

Types of checks:
- Visual check of yield curve to EIOPA input
- Compare spot curve return with the deflator asset
- Compare total-return index return vs deflator asset

#### Notebook 2: Validation of stochastic curves of a risk-neutral output
Purpose:
- Verify if the deterministic curves are consistent with the stochastic curves and if the stochastic curves have the mathematical properties expected from a risk-neutral ESG curves are internally consistent

Types of checks
- Is the mean of the stochastic deflator equal to deterministic curve
- Is the forward return equal to the equivalent deflator return
- Would a buy-and-hold investment strategy return as much as the deflator
- Is the mean spot rate return equal to the deflator return
- is the return of the total-return index equal to deflator return

#### Notebook3: Validation of deterministic and stochastic curves of a real-world output
- To be released
________________________________________
## Contributing
Contributions are welcome! If you have any ideas, bug reports, or suggestions:
1.	Fork the repository.
2.	Create a new branch.
3.	Make your changes and commit them: git commit -m "Add some feature".

________________________________________
## Licence
The notebooks are released under a MIT license. Free to copy, download, modify and use in other products. 
________________________________________
## Disclaimer
No Warranties: This software is provided on an “as is” basis, without warranties or conditions of any kind, either express or implied. The authors do not assume any responsibility for the correct functioning of the code, for any bugs or for unintended consequences arising from the use of this software. Use at your own risk.
________________________________________
Happy validating! If you have questions, suggestions, or concerns, reach out to gregor@osmodelling.com.
