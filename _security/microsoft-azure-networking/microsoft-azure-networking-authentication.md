---
api_key_in: []
api_specs:
- filename: microsoft-azure-networking-backend-address-pools-api-openapi.yml
  format: yaml
  label: Azure Networking Backend Address Pools API
  slug: microsoft-azure-networking-backend-address-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-backend-address-pools-api-openapi.yml
- filename: microsoft-azure-networking-load-balancer-probes-api-openapi.yml
  format: yaml
  label: Azure Networking Load Balancer Probes API
  slug: microsoft-azure-networking-load-balancer-probes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-load-balancer-probes-api-openapi.yml
- filename: microsoft-azure-networking-load-balancers-api-openapi.yml
  format: yaml
  label: Azure Networking Load Balancers API
  slug: microsoft-azure-networking-load-balancers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-load-balancers-api-openapi.yml
- filename: microsoft-azure-networking-load-balancing-rules-api-openapi.yml
  format: yaml
  label: Azure Networking Load Balancing Rules API
  slug: microsoft-azure-networking-load-balancing-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-load-balancing-rules-api-openapi.yml
- filename: microsoft-azure-networking-operations-api-openapi.yml
  format: yaml
  label: Azure Networking Operations API
  slug: microsoft-azure-networking-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-operations-api-openapi.yml
- filename: microsoft-azure-networking-subnets-api-openapi.yml
  format: yaml
  label: Azure Networking Subnets API
  slug: microsoft-azure-networking-subnets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-subnets-api-openapi.yml
- filename: microsoft-azure-networking-virtual-network-peerings-api-openapi.yml
  format: yaml
  label: Azure Networking Virtual Network Peerings API
  slug: microsoft-azure-networking-virtual-network-peerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-virtual-network-peerings-api-openapi.yml
- filename: microsoft-azure-networking-virtual-networks-api-openapi.yml
  format: yaml
  label: Azure Networking Virtual Networks API
  slug: microsoft-azure-networking-virtual-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/openapi/microsoft-azure-networking-virtual-networks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Networking Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Networking secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Networking
provider_slug: microsoft-azure-networking
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: OAuth2Auth
  sources:
  - openapi/azure-networking-load-balancer-openapi.yml
  - openapi/azure-networking-virtual-networks-openapi.yml
  - openapi/microsoft-azure-networking-openapi.yml
  type: oauth2
slug: microsoft-azure-networking-authentication
source_filename: microsoft-azure-networking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-networking-load-balancer-openapi.yml, openapi/azure-networking-virtual-networks-openapi.yml,\n  openapi/microsoft-azure-networking-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/azure-networking-load-balancer-openapi.yml\n  - openapi/azure-networking-virtual-networks-openapi.yml\n  - openapi/microsoft-azure-networking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-networking/refs/heads/main/authentication/microsoft-azure-networking-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
---
