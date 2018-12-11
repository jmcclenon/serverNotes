## Install Jupyter Server on Ubuntu 16.04
![Jupyter Notebooks](https://content-calpoly-edu.s3.amazonaws.com/cosam/1/images/Project%20Jupyter%20logo.png)

1. Create Ubuntu server on AWS with at least 30Gb EBS storage and 2 GB of RAM.

2. Associate elastic IP with the new VM

3. `cd /tmp`

4. `curl -O https://repo.continuum.io/archive/Anaconda3-5.2.0-Linux-x86_64.sh` (lookup most recent version)

5. `bash Anaconda3-5.2.0-Linux-x86_64.sh`


5a. Delete Anaconda3-5.2.0-linux-x86_64.sh when it is finished installing. This is a BIG .sh file.

6. Approve license and path

7. Approve Prepend PATH suggested

```
conda update -n base conda
```
```
conda update anaconda
```
8. Activate installation with: 

```
    source ~/.bashrc
```
9. Create Python3 Environment

```
 conda create --name Python3 python3
```
10. Activate the Python3 Environment 

```
source activate Python3
```

11. Install Numpy, Pandas, etc.

```
conda install numpy, pandas, scikit-learn, plotly, matplotlib
```
Configure the Python2.7 environment (if needed):

```
conda create -n py27 python=2.7
```

```
source activate py27
```
```
conda install notebook ipykernel
```
```
ipython kernel install --user
```

---
To start Jupyter Notebook, use:

```
jupyter notebook --no-ip --port 8888 --no-browser
```
---
To start Jupyter Lab, use:

```
jupyter lab --no-ip --port 9999 --no-browser	
```
Note that the terminal you are running Jupyter Notebook server (or Jupyter Lab server) from will be fully engaged. You will need to start another remote session
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI5Nzc4NzI0NywtMjEwNzEyNDc4MV19
-->