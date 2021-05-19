# Deploy wordpress with MySQL on GKE
This project is intended to deploy wordpress and MySQL using Google Kubernetes Engine

## Starting 🚀
This instructions will help you to get a copy of the project in your host with the purpose of test

## Pre-requisites 📋

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
    c. Run `gcloud init` to initialize the SDK
    ```shell
    ./google-cloud-sdk/bin/gcloud init
    ```
    d. Let's obtain info about our configuration
    ```shel
    ./google-cloud-sdk/bin/gcloud config list
    ```