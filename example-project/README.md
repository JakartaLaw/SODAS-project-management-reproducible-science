# Example project

# Info

This data analysis in this work, does not constitute a real analysis, rather I try to show the different steps of cleaning and analysis data, as usually performed.

# Data

The data is downloaded from: https://projects.fivethirtyeight.com/polls/

using: presidential general election (past cycles)

# Exporting an environment

`conda env export > environment.yml`

And installing environment

`conda env create -f environment.yml`

# Running code

First activate the Conda environment: `conda activate sodas-reproducible-project`

Second, run the code and compile the latex document: `make`. If you do not wish to compile the latex, but just run all code: `make run-code`.

You can run subset of the code by using the commands in the Makefile.