---
api_key_in: []
api_specs:
- filename: virtualMachines.json
  format: json
  label: Azure Virtual Machines REST API
  slug: azure-virtual-machines-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/compute/resource-manager/Microsoft.Compute/ComputeRP/stable/2023-09-01/virtualMachines.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Virtual Machines Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Virtual Machines secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Virtual Machines
provider_slug: microsoft-azure-virtual-machines
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: OAuth2Auth
  sources:
  - openapi/azure-virtual-machines-openapi.yml
  type: oauth2
slug: microsoft-azure-virtual-machines-authentication
source_filename: microsoft-azure-virtual-machines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-virtual-machines-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/azure-virtual-machines-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-virtual-machines/refs/heads/main/authentication/microsoft-azure-virtual-machines-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
---
