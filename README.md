# MICROK8S 101 (Minimal K8S cluster)

This repository intends to be an educational repository for learning microk8s. I use it myself in my private cluster at home, but it's not for working production. It explains how to install, setup and use [microk8s](https://microk8s.io/) a minimal kubernetes cluster orquestator.

## Dependencies.

The following dependencies are required to have microk8s up and running:

- Operating System: Ubuntu v21.10.
- Infrastructure: Raspberry Pi 4 8GB ARM64.
- Domain: Public domain available for TLS encryption.

## installation and setup.

Installation and setup steps are described in the following file [Installation & setup docs](https://github.com/hector-medina/microk8s-101/blob/main/docs/1.%20Installation%20and%20setup.md)

## Services.

There are a couple of services that are pre-configured in this repository. You can find how to deploy them in the docs attached to each service:

### Nextcloud.

It provides a fully-functional private cloud to store your data at home. Let's say it's like a Google Drive like piece of software. For deploying nextcloud run the following command:

```
microk8s kubectl apply -f apps/nextcloud/
```

You can find more info at [setting up nextcloud docs](https://github.com/hector-medina/microk8s-101/blob/main/docs/2.%20Nextcloud.md)
