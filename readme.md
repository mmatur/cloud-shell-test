# Google cloud shell

[![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/mmatur/cloud-shell-test&tutorial=readme.md&cloudshell_workspace=.)

## Starting a local cluster

Our sample application is already available to you. Let's run it on minikube, a local Kubernetes cluster available by default in Cloud Shell, giving you the same experience as deploying to Kubernetes without needing infrastructure:

- In your terminal, run the command below:
```bash
minikube start
```
- If prompted, authorize Cloud Shell to make Google Cloud API calls
- Once your local cluster in Cloud Shell is set-up, you will see the following message
```
* Done! kubectl is now configured to use "minikube" cluster and "default" namespace by default
```
- Check the minikube cluster is running
```bash
kubectl get nodes
```

## Let's now run this app:

- Click `Cloud Code` in the status bar

- Select `Run on Kubernetes`, confirm that you want to use the "minikube" context

- An Output panel will pop-up after a few seconds, displaying the progress as your app is built/deployed

- Once your app is built, launch it with the Web Preview link displayed in your Output panel, near the text:
```bash
Forwarded URL from service traefik:
```

## Let's install the powpow Agent now

- Create an account on https://powpow.traefik.io

![Login](https://user-images.githubusercontent.com/1776972/134343608-adb7e547-b015-44b9-b117-2a67968de64e.png)

- On the dashboard page, click on `Connect Cluster`

![Home](https://user-images.githubusercontent.com/1776972/134343607-3d79417c-cbc7-4231-8c09-8c3d27454aa5.png)

- Set a name for your cluster, and click on `Save and Continue`

![Create cluster](https://user-images.githubusercontent.com/1776972/134343604-384b8d38-7a3c-4af7-881c-4e30b439ebba.png)

- Follow setps to install the powpow agent

![Install agent](https://user-images.githubusercontent.com/1776972/134343598-45ef953a-2200-4e50-a3ae-07ade571caeb.png)

- Check the results

![Ingresses](https://user-images.githubusercontent.com/1776972/134343587-2c58ed8f-01d9-45bb-a32b-2f35cbc5feed.png)
