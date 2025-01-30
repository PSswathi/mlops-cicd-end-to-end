# mlops-cicd-end-to-end

AWS-CICD-Deployment-with-Github-Actions
1. Login to AWS console.
2. Create IAM user for deployment
#with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess



##3. Create ECR repo to store/save docker image

ECR repository name :

309166109941.dkr.ecr.us-east-1.amazonaws.com/mlops-end-end-project

start running

try ci cd

##Runner actions

mkdir actions-runner

cd actions-runner

url -o actions-runner-linux-x64-2.321.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.321.0/actions-runner-linux-x64-2.321.0.tar.gz

echo "ba46ba7ce3a4d7236b16fbe44419fb453bc08f866b24f04d549ec89f1722a29e  actions-runner-linux-x64-2.321.0.tar.gz" | shasum -a 256 -c

tar xzf ./actions-runner-linux-x64-2.321.0.tar.gz

./config.sh --url https://github.com/PSswathi/mlops-cicd-end-to-end --token BFMPKK4LRVNFMKFO22RLPGDHTPQN6


./run.sh

After  this we see connected to github


