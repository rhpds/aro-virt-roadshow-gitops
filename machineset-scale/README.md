# machineset-scale - takes a number of machines, spreads across machinesets

This repository contains a Helm chart

## Overview

When used with an ArgoCD Application, this Helm chart provides the following functionalities:

* assumes three users per Stadard_D16s_v3 Azure instance type
* kubevirt needs the same cpu-model to do LiveMigration
* machinesets differ in cpu-model, even if Azure instance type is the same (e.g. Standard_D4s_v3)
* this chart scales the machinesets evenly to 3 + num_users * .3 and rounds up to int

## Usage

## Prerequisites

- **ArgoCD**: Make sure you have ArgoCD installed and configured in your OpenShift cluster.
