For the OpenAI configuration for Aure lightspeed, the KCS has been used.
KCS used : https://access.redhat.com/solutions/7099270


OpenShift Lightspeed - Azure OpenAI Integration

This contains the configuration files needed to integrate Red Hat OpenShift Lightspeed with Azure OpenAI using a hardcoded API token.

## 🔧 Overview

The setup allows OpenShift Lightspeed to connect with an Azure-hosted GPT model (`gpt-4.1-nano`) using a registered Azure OpenAI deployment.

## 📂 Files

- `azure-api-keys-secret.yaml`: Kubernetes `Secret` containing the API token and endpoint information required to authenticate with Azure OpenAI.
- `olsconfig.yaml`: OLSConfig CRD configuring Lightspeed to use the Azure model via the credentials in the secret.

---

## 🔑 Prerequisites

- You must have:
  - A valid Azure OpenAI deployment
  - Access to the OpenShift cluster with `openshift-lightspeed` namespace
  - Your Azure OpenAI API Key

---
