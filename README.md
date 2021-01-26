# Realtime LnL on Knative and Apache Yunikorn

This repo demonstrates how to use Knative to make working with Kubernetes clusters a
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