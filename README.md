# PythonK8client
[Kubernetes](https://kubernetes.io) Library for [Python](https://www.python.org) - [minikube](https://minikube.sigs.k8s.io/) 

### Purpose:
Kubernetes Python client is used to perform operations on Kubernetes resources in the cluster from your Python code.

### Setup and instructions:

- **Pre-requisite**:  A Running Kubernetes Cluster is required. (Note: I am using **minikube** cluster on macOS:  `brew install minikube`)
- **Create** and ***activate*** **venv**:
  1. `python3 -m venv <srcdir>` *(path to PythonK8sClient)*
  2. `source <srcdir>/bin/activate`
- *With **activated** environment* install Kubernetes client for Python 3 with **pip3** by using command: `pip3 install kubernetes`. 
- kubectl utility to verify the resources, such as `kubectl`, such as.
- (optional) create `.gitignore` be sure to include:
  - `bin/`
  - `lib/`
  - `include/`

### run

* Test by running `python3 knodes.py`
* To deactivate venv:  `deactivate`

TODO
* conda
- - -
## conda notes

### Link:
[Managing environments — conda 24.1.3.dev68 documentation](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#activating-an-environment)

### To create and activate an environment: 
#### Set *$myenv* to repo name and create new Conda environment :

```sh
myenv=`basename "$PWD"`
conda create --name $myenv -y
conda activate $myenv
```

### Installing Kubernetes 
**Link**:  [kubernetes-feedstock/README.md at main · conda-forge/kubernetes-feedstock](https://github.com/conda-forge/kubernetes-feedstock/blob/main/README.md#installing-kubernetes)

**Github b** repo:
[conda-forge/kubernetes-feedstock: A conda-smithy repository for kubernetes.](https://github.com/conda-forge/kubernetes-feedstock.git)

```sh
conda config --add channels conda-forge
conda config --set channel_priority strict
#
conda install kubernetes kubernetes-client kubernetes-node kubernetes-server -y
conda install python-kubernetes -y

python3 knodes.py
```

##### for macOS and Linux:  Locate the directory for the conda environment in your terminal window by running in the terminal echo $CONDA_PREFIX.
##### Enter that directory and create these subdirectories and files:
```sh
cd $CONDA_PREFIX
mkdir -p ./etc/conda/activate.d
mkdir -p ./etc/conda/deactivate.d
touch ./etc/conda/activate.d/env_vars.sh
touch ./etc/conda/deactivate.d/env_vars.sh

##### Edit ./etc/conda/activate.d/env_vars.sh as follows:
```sh
#!/bin/sh

export MY_KEY='secret-key-value'
export MY_FILE=/path/to/my/file/
```

##### Edit ./etc/conda/deactivate.d/env_vars.sh as follows:
```sh
#!/bin/sh

unset MY_KEY
unset MY_FILE
```

> When you run conda activate analytics, the environment variables MY_KEY and MY_FILE are set to the values you wrote into the file. When you run conda deactivate, those variables are erased.

##### Export your active environment to a new file:
```bash
conda env export > environment.yml
```

- - -
#python
#kubernetes
#github 
- - -
### Mar 20, 2024
##### This is a selfie my daughter H (*Mika*) took this morning after she woke up in Japan today!![](732593856.jpg)
 👧❤️🇯🇵

#japan 
- - -
### My Animal Crossing island!  It is called:
### 64^2
![](IMG_3801.jpeg)


#animalcrossing
