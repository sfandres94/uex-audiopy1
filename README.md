# uex-audiopy
This repository has been created for the lab session on audio processing with Python of the Multimedia Systems subject at the University of Extremadura (UEx).

# First steps

Check if Anaconda is installed:
```
conda --version
conda -V
```
otherwise install it according to https://docs.anaconda.com/anaconda/install/index.html

Create the conda environment from the environment.yml file:
```
conda env create -f environment.yml
```

Activate the conda environment:
```
conda activate <env_name>
```
where `<env_name>` is the name of the conda environment we have just created. It appears in the first line of the environment.yml file, `audiopy-conda` in this particular case.

Add the conda environment to Jupyter lab so that it appears as a kernel:
```
python3 -m ipykernel install --user --name=audiopy-conda
```

Check that the kernel has been installed correctly:
```
jupyter kernelspec list
```

Now we can run Jupyter lab and select `audiopy-conda` as the running kernel:
```
jupyter-lab
```
