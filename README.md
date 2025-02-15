# flask-login-app
# Powershell

mkdir C:\Users\user\lambda_package
cd C:\Users\user\lambda_package
pip install --no-user requests PyGithub cryptography -t .
Compress-Archive -Path * -DestinationPath C:\Users\user\lambda_function.zip -Force

# Sometimes you need to make files from linux os only, cause cryptography is linux compatible

so, get a docker into vscode and try or else, create a linux free tier ec2 and give these commands one by one

# Update package list
sudo yum update -y

# Install Python 3 and pip
sudo yum install -y python3 python3-pip

# Verify pip3 is installed
pip3 --version

# Step 1: Create a directory for Lambda package
mkdir lambda_package && cd lambda_package

# Step 2: Install required Python dependencies
pip3 install requests PyGithub cryptography -t .

# Step 3: Zip the installed dependencies
zip -r lambda_function.zip .

# From your local system, try this 
scp -i "C:\Users\manoj.kamatam\Downloads\Dev-AIIntegration.pem" ec2-user@34.229.146.117:/home/ec2-user/lambda_package/lambda_function.zip C:\Users\manoj.kamatam\Downloads\ 
