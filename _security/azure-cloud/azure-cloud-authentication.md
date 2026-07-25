---
api_key_in: []
api_specs:
- filename: azure-cloud-availability-sets-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cloud Availability Sets API
  slug: azure-cloud-availability-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cloud/refs/heads/main/openapi/azure-cloud-availability-sets-api-openapi.yml
- filename: azure-cloud-disks-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cloud Disks API
  slug: azure-cloud-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cloud/refs/heads/main/openapi/azure-cloud-disks-api-openapi.yml
- filename: azure-cloud-snapshots-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cloud Snapshots API
  slug: azure-cloud-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cloud/refs/heads/main/openapi/azure-cloud-snapshots-api-openapi.yml
- filename: azure-cloud-virtual-machine-scale-sets-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cloud Virtual Machine Scale Sets API
  slug: azure-cloud-virtual-machine-scale-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cloud/refs/heads/main/openapi/azure-cloud-virtual-machine-scale-sets-api-openapi.yml
- filename: azure-cloud-virtual-machines-api-openapi.yml
  format: yaml
  label: Microsoft Azure Cloud Virtual Machines API
  slug: azure-cloud-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cloud/refs/heads/main/openapi/azure-cloud-virtual-machines-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Azure Cloud secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Azure Cloud
provider_slug: azure-cloud
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://management.azure.com/.default)
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  sources:
  - openapi/azure-cloud-openapi.yml
  type: oauth2
slug: azure-cloud-authentication
source_filename: azure-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-cloud-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: entra\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token (scope https://management.azure.com/.default)\n  sources:\n  - openapi/azure-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-cloud/refs/heads/main/authentication/azure-cloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI
- Cloud Computing
- Databases
- IaaS
- Infrastructure
- Machine Learning
- Microsoft
- Networking
- PaaS
- Platform as a Service
- SaaS
- Storage
---
