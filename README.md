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

#python
#kubernetes
#github 

