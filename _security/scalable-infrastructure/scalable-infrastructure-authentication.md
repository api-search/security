---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS EC2 API
  slug: aws-ec2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/amazonaws.com/ec2/2016-11-15/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: AWS VPC API
  slug: aws-vpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/amazonaws.com/ec2/2016-11-15/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: AWS EKS API
  slug: aws-eks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/amazonaws.com/eks/2018-08-23/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Google Compute Engine API
  slug: google-compute-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/googleapis.com/compute/v1/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Google Kubernetes Engine API
  slug: google-kubernetes-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/googleapis.com/container/v1/openapi.yaml
- filename: resources.json
  format: json
  label: Azure Resource Manager API
  slug: azure-resource-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/resources/resource-manager/Microsoft.Resources/stable/2023-07-01/resources.json
- filename: managedClusters.json
  format: json
  label: Azure AKS API
  slug: azure-aks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/containerservice/resource-manager/Microsoft.ContainerService/aks/stable/2024-01-01/managedClusters.json
- filename: DigitalOcean-public.v2.yaml
  format: yaml
  label: DigitalOcean API
  slug: digitalocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/digitalocean/openapi/main/specification/DigitalOcean-public.v2.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scalable Infrastructure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalable Infrastructure secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalable Infrastructure
provider_slug: scalable-infrastructure
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed request (Authorization header).
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/scalable-infrastructure-openapi.yml
  type: apiKey
slug: scalable-infrastructure-authentication
source_filename: scalable-infrastructure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalable-infrastructure-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed request (Authorization header).\n  sources:\n  - openapi/scalable-infrastructure-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-infrastructure/refs/heads/main/authentication/scalable-infrastructure-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Infrastructure
- Compute
- DevOps
- Infrastructure as Code
- Kubernetes
- Networking
- Scalability
- Storage
---
