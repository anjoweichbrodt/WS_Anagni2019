# Step-by-step Preparations

**1. Install COMPAS**

> **Note**
> <br />
> For the following, on Windows, use the Anaconda Prompt (launched as administrator), not the Command Prompt.
> <br />On Mac, use the Terminal.

To install COMPAS, simply type the following on the command line

```bash
conda install -c conda-forge COMPAS
```

To check the installation, simply try to import the core COMPAS packages in the interactive Python interpreter.

```python
>>> import compas
>>> import compas_rhino
>>> import compas_ghpython
>>> import compas_blender
>>> import compas_plotters
>>> import compas_viewers
>>> exit()
```

**2. Install support packages**

> **Note**
> <br />
> For the following, on Windows, use the Anaconda Prompt (launched as administrator), not the Command Prompt.
> <br />On Mac, use the Terminal.

To install the required support packages, simply type the following on the command line

```bash
conda install -c conda-forge shapely
conda install -c conda-forge cvxopt
conda install -c cvxgrp cvxpy
conda install -c IBMDecisionOptimization cplex
```

To check the installation, try importing the packages in the interactive Python interpreter

```python
>>> import shapely
>>> import cvxopt
>>> import cvxpy
>>> import cplex
>>> exit()
```

**3. Install additional COMPAS packages**

> **Note**
> <br />
> For the following, on Windows, use the Anaconda Prompt (launched as administrator), not the Command Prompt.
> <br />On Mac, use the Terminal.

To install the additional COMPAS packages, simply type the following on the command line

```bash
pip install -e git+https://github.com/BlockResearchGroup/compas_tna.git
pip install -e git+https://github.com/BlockResearchGroup/compas_assembly.git
pip install -e git+https://github.com/BlockResearchGroup/compas_rbe.git
```

To check the installation, import the packages in the interactive Python interpreter

```python
>>> import compas_tna
>>> import compas_assembly
>>> import compas_rbe
>>> exit()
```
