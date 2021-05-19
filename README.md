# Deploy wordpress with MySQL on GKE
This project is intended to deploy wordpress and MySQL using Google Kubernetes Engine

## Starting 🚀
This instructions will help you to get a copy of the project in your host with the purpose of test

## Pre-requisites 📋

- Web browser
- Linux or macOS or Windows
- Kubernetes
- Google Cloud SDK
- Bash for Windows (git bash should suffice)

## Installation 🔧

### Installing Google Cloud SDK

1. Cloud SDK requires Python; supported versions are Python 3 (preferred, 3.5 to 3.8) and Python 2 (2.7.9 or higher).

    Check your python version
    ```shell
    python -v
    ```
2. Download the Google Cloud SDK
    ```shell
    wget https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-341.0.0-darwin-x86_64.tar.gz
    ```

    a. Extract the archive file
    ```shell
    tar -xvf google-cloud-sdk-341.0.0-darwin-x86_64.tar.gz
    ```
    b. Run the script
    ```shell
    ./google-cloud-sdk/install.sh
    ```
    c. Export the path
    ```shell
    export PATH=~/google-cloud-sdk/bin:$PATH 
    ```
    d. Run `gcloud init` to initialize the SDK
    ```shell
    gcloud init
    ```
    e. Let's obtain info about our configuration
    ```shell
    gcloud config list
    ```

### Installing Kubernetes

1. Download the latest version
    ```shell
    wget https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl
    ```
2. Set the execution permissions of the kubectl binary
    ```shell
    chmod +x ./kubectl
    ```
3. Move the binary into your PATH.
    ```shell
    mv ./kubectl /usr/local/bin/kubectl
    ```
4. Check if the most recent version has been installed
    ```shell
    kubectl version --client
    ```