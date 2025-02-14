# flask-login-app
# Powershell >

mkdir C:\Users\user\lambda_package
cd C:\Users\user\lambda_package
pip install --no-user requests PyGithub cryptography -t C:\Users\user\lambda_package
Compress-Archive -Path C:\Users\user\lambda_package\* -DestinationPath C:\Users\user\lambda_function.zip -Force
