# localstack
Deploying [LocalStack](https://localstack.cloud/) ( A fully functional local cloud stack ) on Vagrant with the help of ansible as a provisioner

### How to use
```bash
git clone https://github.com/theJaxon/localstack.git

cd localstack && vagrant up

# Create the needed terraform files in this directory which maps to /vagrant on the guest machine
```

---

### Tools Included
- [**tflocal**](https://github.com/localstack/terraform-local) -  Terraform CLI wrapper to deploy your Terraform applications directly to LocalStack
- [**awslocal** (aliased to aws)](https://github.com/localstack/awscli-local) - Thin wrapper around the "aws" command line interface for use with LocalStack 
- [**DynamoDB Admin**](https://www.npmjs.com/package/dynamodb-admin) - GUI for DynamoDB Local, dynalite, localstack etc.
