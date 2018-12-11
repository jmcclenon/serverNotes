## Install Jupyter Server on Ubuntu 16.04
![Jupyter Notebooks](https://content-calpoly-edu.s3.amazonaws.com/cosam/1/images/Project%20Jupyter%20logo.png)

1. Create Ubuntu server on AWS with 30Gb EBS storage

2. Associate elastic IP to the new server

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
9. 

 conda create --name Python3 python3

11. source activate Python3

12. conda install numpy, pandas, scikit-learn, plotly, matplotlib... etc.

configure the python2.7 environment:

conda create -n py27 python=2.7

source activate py27

conda install notebook ipykernel

ipython kernel install --user
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTY2MzY1NTgsLTIxMDcxMjQ3ODFdfQ==
-->