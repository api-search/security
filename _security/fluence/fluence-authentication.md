---
api_key_in:
- header
api_specs:
- filename: fluence-billing-api-openapi.yml
  format: yaml
  label: Fluence Billing API
  slug: fluence-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-billing-api-openapi.yml
- filename: fluence-hardware-api-openapi.yml
  format: yaml
  label: Fluence Hardware API
  slug: fluence-hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-hardware-api-openapi.yml
- filename: fluence-prices-api-openapi.yml
  format: yaml
  label: Fluence Prices API
  slug: fluence-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-prices-api-openapi.yml
- filename: fluence-publicip-api-openapi.yml
  format: yaml
  label: Fluence PublicIP API
  slug: fluence-publicip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-publicip-api-openapi.yml
- filename: fluence-securitygroup-api-openapi.yml
  format: yaml
  label: Fluence SecurityGroup API
  slug: fluence-securitygroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-securitygroup-api-openapi.yml
- filename: fluence-service-api-openapi.yml
  format: yaml
  label: Fluence Service API
  slug: fluence-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-service-api-openapi.yml
- filename: fluence-ssh-keys-api-openapi.yml
  format: yaml
  label: Fluence SSH keys API
  slug: fluence-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-ssh-keys-api-openapi.yml
- filename: fluence-storage-api-openapi.yml
  format: yaml
  label: Fluence Storage API
  slug: fluence-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-storage-api-openapi.yml
- filename: fluence-subnets-api-openapi.yml
  format: yaml
  label: Fluence Subnets API
  slug: fluence-subnets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-subnets-api-openapi.yml
- filename: fluence-users-api-openapi.yml
  format: yaml
  label: Fluence Users API
  slug: fluence-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-users-api-openapi.yml
- filename: fluence-vms-api-openapi.yml
  format: yaml
  label: Fluence VMs API
  slug: fluence-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-vms-api-openapi.yml
- filename: fluence-vpcs-api-openapi.yml
  format: yaml
  label: Fluence VPCs API
  slug: fluence-vpcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/openapi/fluence-vpcs-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fluence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fluence secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fluence
provider_slug: fluence
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token issued by Fluence
  name: access_jwt_token
  scheme: bearer
  sources:
  - openapi/fluence-openapi-original.yml
  type: http
- in: header
  name: api_key
  parameter: X-API-KEY
  sources:
  - openapi/fluence-openapi-original.yml
  type: apiKey
slug: fluence-authentication
source_filename: fluence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fluence-openapi-original.yml\ndocs: https://fluence.dev/docs/build/api/overview\nnotes: >-\n  Primary auth is an API key sent in the X-API-KEY header (create/manage at\n  console.fluence.network/settings/api-keys); a missing or invalid key returns forbidden.\n  A JWT bearer token (access_jwt_token) is used for console/session flows. API keys carry\n  permission scopes — see scopes/fluence-scopes.yml.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: access_jwt_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token issued by Fluence\n  sources:\n  - openapi/fluence-openapi-original.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/fluence-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluence/refs/heads/main/authentication/fluence-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Crypto Web3
- Cloud Compute
- DePIN
- GPU
- Infrastructure
- Virtual Machines
- AI Infrastructure
- Decentralized Cloud
---
