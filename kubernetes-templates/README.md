## kubernetes-templates

This directory contains exemplary templates of how to run XAP data grid with existing [Kubernetes cluster](https://github.com/kubernetes/kubernetes/blob/master/docs).

### Pre-requirements

1. [Docker registry](https://docs.docker.com/registry/deploying/), that stores XAP docker image

2. Kubernetes cluster that might be running locally, on-premises VMs or on a cloud provider

3. Linux box with installed 

    - Make Utility
    - [kubectl](https://kubernetes.io/docs/user-guide/prereqs/) should be connected to the kubernetes cluster

### Usage

> Edit Makefile with correct parameter values.

#### Create XAP [pull image secret](https://kubernetes.io/docs/user-guide/images/)

    make create-image-pull-secret

#### Create XAP IMDG
    
    make create-xap-datagrid
  