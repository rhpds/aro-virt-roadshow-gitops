# roadshow-vms - deploy the roadshow-vms

## Overview

When used with an ArgoCD Application, this Helm chart provides the following functionalities:

.VMs
. database
. winweb01
. winweb02

. Sets up NodeSelectors on every vm if desired

. VMs expect datavolumes to be in the default namespace

## Usage

## Prerequisites

- **ArgoCD**: Make sure you have ArgoCD installed and configured in your OpenShift cluster.
