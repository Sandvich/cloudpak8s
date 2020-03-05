---
title: cp4i-on-roks
weight: 300
---

## Introduction

This page describes all the steps on how to deploy the Integration Cloud Pak to managed openshift on IBM cloud.  This requires a paid IBM Cloud Account with the ability to create Red Hat Open Shift clusters.  It also requires a license for which can be used to deploy the Cloud Pak for Integration.

## Deploy a managed OpenShift Cluster on IBM Cloud

1. Log into your IBM Cloud Account.  From the Dashboard on the Search Bar, enter in `Cloud Pak for Integration`.  It will take you to the section where you can create your own cluster.

2. Follow these steps to deploy Red Hat Open Shift and the Common Services -- [here](https://cloud.ibm.com/docs/cloud-pak-integration?topic=cloud-pak-integration-getting-started)
3. After you complete the installation process it will create some default namespaces as well as apply some general security required to install the cloud pak.  It will also automatically create a `Pull Secret` for you that you can use to deploy capabilities.  This secret is called `ibm-entitlement-key` and will be referenced multiple times.

## Deploy Capabilities

We recommend that you deploy Tracing before any of the other components.

- [Tracing](../deploy-tracing)
- [App Connect](../deploy-integration)
- [API Connect](../deploy-api-mgmt)
- [MQ](../deploy-queue-manager)
- [Event Streams](../deploy-eventstreams)
- [Aspera](../deploy-fast-file-transfer)
- [DataPower](../deploy-secure-gateway)
- [Asset Repository](../deploy-asset-repo)
