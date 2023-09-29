# LiAPI Helm Chart

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installing the Chart](#installing-the-chart)
- [Uninstalling the Chart](#uninstalling-the-chart)
- [Configuration](#configuration)

## Overview

This Helm Chart is designed to deploy the LiAPI application on a Kubernetes cluster. This README provides guidelines on how to configure, install, and manage the Helm Chart for different environments.

## Prerequisites

- Helm v3.0+
- Kubernetes 1.16+

## Installing the Chart

To install the chart with the release name `liapi`, run the following:

```bash
helm install liapi . --values values.yaml
```

Replace `values.yaml` with the path to the configuration file containing your customized values. For current values available for the liapi helm chart, visit the [Liapi README](charts/liapi/README.md)

## Using the repo

Charts are released when the Chart.yaml file's version parameter has been updated and pushes to main occur.

If you'd like to use the latest chart:

```bash
helm repo add liapi https://caylorinc.github.io/liapi-charts/
helm repo update
helm install liapi liapi/liapi --values values.yaml
```

## Uninstalling the Chart

To uninstall or delete the `liapi` deployment:

```bash
helm uninstall liapi
```

## Upgrading

To upgrade the `liapi` deployment with a new version of the chart or configuration:

```bash
helm upgrade liapi . --values values.yaml
```


### Note

This README provides essential documentation for configuring, installing, and managing the Helm Chart for LiAPI. For more detailed information, please refer to the official Helm documentation.