# ArgoCD-PG-Deploy

## Overview

All the necessary yaml files to deploy prometheus (server) and grafana in kubernetes

## Folder structure

The folder structure is as follows :

```bash

      --- environments
      |     |
      |     --- overlays
      |           |
      |           --- prod
      |                 |
      |                 --- namespace
      |                 |     |
      |                 |     --- limit-range.yaml
      |                 |     --- namespace.yaml
      |                 |     --- resource-quota.yaml
      |                 --- shared
      |                 |     |
      |                 |     --- shared-resousrce (i.e pv)
      |                 |
      |                 --- kustermization.yaml
      |
      --- manifests
            |
            --- services
                  |
                  |
                  --- base
                        |
                        --- grafana-dashboards-configmap.yaml
                            grafana-dashboard-node-cluster-configmap.yaml
                            pormetheus-configmap.yaml
                            secrets.yaml
                            serviceaccount.yaml
                            prometheus-deploy.yaml
                            grafana-service.yaml
                            grafana-deploy.yaml
                            renderer-service.yaml
                            rendrer-deploy.yaml
                            kustomization.yaml

```
            

