# [Historic_Masonry_Anagni_2019](http://www.block.arch.ethz.ch/brg/teaching/historic-masonry-summer-school-anagni-2019)
International Summer School on Historic Masonry - Anagni 2019

![img](Tools/masonry_structures_school_2019_anagni-logo-e1547807560485_1550829849_1920x1080.png)

General website: [https://historicmasonryschool2019.wordpress.com/](https://historicmasonryschool2019.wordpress.com/)


## BRG Day 1: Tuesday 18/06/2019
   * Part 1 (12.30 - 13.30)
      * Overview Lecture: compas_masonry
   
   * Part 2 (17.00 - 17.30)
      * Thrust Network Analysis (TNA) - [Theory](Theory/TNA)
      
   * Part 3 (17.30 - 19.00)
      * Thrust Network Analysis (TNA) - tutorial


## BRG Day 2: Wednesday 19/06/2019
   * Part 1 (13.00 - 13.30)
      * Discrete Element Modeling (DEM) - theory

   * Part 2 (15.00 - 16.00)
      * Discrete Element Modeling (DEM) - tutorial

   * Part 3 (16.00 - 16.30)
      * Rigid Block Equilibrium (RBE) - theory

   * Part 4 (17.00 - 18.00)
      * Rigid Block Equilibrium (RBE) - tutorial     

   * Part 5 (18.00 - 19.00)
      * Piece-wise Rigid Displacements (PRD) - tutorial   
      
      
## BRG Day 3: Thursday  20/06/2019

   * (16.45 - 18.00)

      *[Lecture](https://www.dropbox.com/s/6sq1ypvg06iaabq/20190110_Tongji_PBlock.pdf?dl=0)* by Prof. Philippe Block at the American Academy in Rome, "Reimagining Shell Structures: Learning from the Master Builders".

 
## Tools
* Installation
  * Software
  
    [Rhino 6 for Windows](https://www.rhino3d.com/it/download/rhino-for-windows/6/evaluation)
    
    [Rhino 5 for Windows](https://www.rhino3d.com/download/rhino/5/latest)
    
    [Rhino for Mac](https://www.rhino3d.com/download/rhino-for-mac/5/evaluation)
 
    [3DEC demo version](https://www.itascacg.com/software-demo)
  
    [Sublime](https://www.sublimetext.com/)



## compas Installation

**Install the latest released version of COMPAS using `conda`**

```bash
conda config --add channels conda-forge
conda install COMPAS
```

**Check your installation**

Launch the interactive Python interpreter and import `compas`, `compas_rhino`, `compas_ghpython`.

```bash
>>> import compas
>>> import compas_rhino
>>> import compas_ghpython
>>> compas.__version__
0.5.1
```

If no error messages appear and the COMPAS version is correct, you're good to go.
Type `exit()` to quit the interpreter.

**Configure your editor**

Detailed instructions can be found here:

*   Sublime Text 3: https://compas-dev.github.io/main/environments/sublimetext.html
*   VS Code: https://compas-dev.github.io/main/environments/vscode.html

Once everything is set up, run `verify_editor.py` to check the setup.
If this prints `0.5.1` in the Terminal window, your editor is properly configured.

**Install COMPAS for Rhino**

To make the installed COMPAS packages available in Rhino run the following on the command line

```bash
python -m compas_rhino.install -v 5.0
```

> **Note** (Windows only)
>
> Use `-v 6.0` instead of `-v 5.0` if you want to use Rhino 6 instead of Rhino 5.

Open Rhino and run `verify_rhino.py`.
If this does not throw an error and prints the correct COMPAS version (`0.5.1`),
Rhino is properly configured.

> **Note**
>
> To run a script in Rhino, just type `RunPythonScript` at the Rhino command prompt
> and select the script you want to run.

