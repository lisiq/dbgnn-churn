FROM pytorch/pytorch:2.4.1-cuda12.1-cudnn9-runtime
WORKDIR /workspaces/pathpyG
RUN apt-get update
RUN apt-get -y install git

# For signed commits: https://code.visualstudio.com/remote/advancedcontainers/sharing-git-credentials#_sharing-gpg-keys
RUN apt install gnupg2 -y

# Install the requirements
COPY requirements.txt .
RUN pip install -r requirements.txt
