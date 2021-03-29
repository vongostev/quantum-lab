# Quantum-lab
Tested on Windows 10 Pro 20H2.

## Environment setup
1. Install anaconda: https://www.anaconda.com/products/individual
2. Open Anaconda Prompt to use a command line with conda

```
$ conda init
```

4. Clone this repo

```
$ git clone https://github.com/vongostev/quantum-lab.git
```

5. Create, activate, and setup env

```
$ conda env create -f environment.yml
$ conda activate quantum-lab 
```

6. Install conda env jupyter-lab kernel

```
$ ipython kernel install --name quantum-lab --display-name Quantum-Lab --user
```

## IBMQ credentials setup
1. Create account on https://quantum-computing.ibm.com/
2. Replace <your token here> string in save_ibmq_token.py with your actual API token from https://quantum-computing.ibm.com/
3. Run save_ibmq_token.py

```
$ python save_ibmq_token.py
```

4. Done. Now you can use following code to access IBMQ:
    
```
import helpers
provider = helpers.get_ibmq_provider()
``` 


## Environment usage after setup
1. Start Jupyter notebook

```
$ jupyter notebook
```

2. Change kernel to "Quantum-Lab"
    
## Useful links
- [Getting started with Qiskit](https://qiskit.org/documentation/getting_started.html)
- [Learn Quantum Computation using Qiskit](https://qiskit.org/textbook)