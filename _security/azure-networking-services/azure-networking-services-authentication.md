---
api_key_in: []
api_specs:
- filename: azure-networking-services-virtual-network-openapi.yaml
  format: yaml
  label: Azure Virtual Networks API
  slug: azure-virtual-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/openapi/azure-networking-services-virtual-network-openapi.yaml
- filename: azure-networking-services-virtual-network-openapi.yaml
  format: yaml
  label: Azure Load Balancer API
  slug: azure-load-balancer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/openapi/azure-networking-services-virtual-network-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Networking Services Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Networking Services secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Networking Services
provider_slug: azure-networking-services
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-networking-services-load-balancer-openapi.yaml
  - openapi/azure-networking-services-virtual-network-openapi.yaml
  type: oauth2
slug: azure-networking-services-authentication
source_filename: azure-networking-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-networking-services-load-balancer-openapi.yaml, openapi/azure-networking-services-virtual-network-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/azure-networking-services-load-balancer-openapi.yaml\n  - openapi/azure-networking-services-virtual-network-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/authentication/azure-networking-services-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
---
