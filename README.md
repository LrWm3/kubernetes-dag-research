# activiti-kubeapps

A project in which I try and get [kubeapps](https://hub.kubeapps.com/) and 
[activiti](https://github.com/Activiti/Activiti) working together, as I think that's an interesting platform.

## To Run

Follow this guide to set up kubeapps: https://github.com/kubeapps/kubeapps/blob/master/docs/user/getting-started.md
Follow this guide to set up activiti: https://activiti.gitbook.io/activiti-7-developers-guide/getting-started/getting-started-activiti-cloud

> I spent a long time dealing with redirect errors with activiti's `modeling-service`. When I edited my host file, I
> used `127.0.0.1`, but I needed to use my machines public IP address. Afterwards it worked properly. I don't know 
> exactly why this was so troublesome but it took me 4 hours to debug, roughly

However it turns out I didn't realy want activiti after all. It was not what I wanted.

## Next up: Argo

[argo](https://github.com/argoproj/argo) seems good

To install: `helm repo add argo https://argoproj.github.io/argo-helm`

### Findings

Argo was cool, but it lacked the ability to set things up quickly in the cluster

## Next up x2: Apache Airflow

Of course an apache product is the best thing I've found so far. [Apache Airflow](https://airflow.apache.org/) has 
more features and better visualization; I think it's possible to create DAG in Airflow, which is what I was hoping for
originally.

## An aside: kubeprod

I was looking for a production-ready kubernetes deployment, and I finally found it; [kubeprod/BKPR](https://kubeprod.io/)

I would like to use this at some point.

