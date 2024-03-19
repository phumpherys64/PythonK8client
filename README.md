# PythonK8client
Kubernetes Library for Python - Minikube examples

### Purpose:
Kubernetes Python client is used to perform operations on Kubernetes resources in the cluster from your Python code.

### Setup and instructions:

- **Pre-requisite**:  A Running Kubernetes Cluster is required. (Note: I am using **minikube** cluster)
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
* etc.
