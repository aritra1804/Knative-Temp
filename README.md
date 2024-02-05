# Knative-Temp

This repository is a boilerplate code for Knative projects. Knative is a Kubernetes-based platform for running serverless. Serverless means you can scale your application to 0 running instances but those instances to quickly scale up to N number of instances within a few seconds. Anyone who wants to use Knative for their projects can use [this repository](https://github.com/aritra1804/Knative-Temp.git) for reference.


## Requirements
- [Terraform](https://developer.hashicorp.com/terraform/downloads) installed
- [Kubectl](https://kubernetes.io/docs/tasks/tools/) installed


## Running the code
### 1. Clone this repo

```
git clone https://github.com/aritra1804/Knative-Temp.git
cd Knative-Temp
```

### 2. Initialize Terraform
Create an account on [Linode](https://www.linode.com/cfe) and get an API Key in your Linode account [here](https://cloud.linode.com/profile/tokens).

Once you have a key, do the following:

```bash
echo "linode_api_token=\"YOUR_API_KEY\"" >> terraform.tfvars
echo "k8s_node_type=\"g6-standard-2\"" >> terraform.tfstate
```

Now run
```bash
terraform init
```

Now you can run the different scripts needed as per requirement to add services to your project.
