# Realtime LnL on Knative and Apache Yunikorn

This repo demonstrates how to use Knative and Apache Yunikorn to make working with Kubernetes clusters a
little less of ops tasks on developers. Knative is a kubernetes based platform to manage
the configuration and deployments of serverless apps.

Yunikorn is an apache project that aims to unleash the power resource scheduling when 
running Big Data or ML applications on Kubernetes. 

### Set up and installation
The prerequisites to use Knative are:

#### Configure Minikube
For testing on dim-down kubernetes install, we recommend using minikube. Make sure to
configure Minikube to run Knative locally in your machine. Run the following commands to 
set the configurations. 

```
$ minikube config set kubernetes-version v1.20.0
$ minikube config set memory 6000
$ minikube config set cpus 4
```

Ensure that these changes take effect by deleting and restarting the minikube cluster

```
$ minikube delete
$ minikube start
```


#### Install and Configure CLI for Knative (`kn`)

In a suitable directory (eg. `mkdir knative-poc`), follow the instructions [here](https://github.com/knative/client/blob/master/docs/README.md)
to install and configure `kn` the knative CLI for your environment


#### Install and Configure Knative on your Kubernetes Cluster

On many kubernetes distributions, one can obtain and install specific operators that simplify the installation of 
Knative on Kubernetes. Example for Openshift, you can install the `RedHat Openshift Serverless` operator to provide 
Knative capabilities on top on Openshift. 

