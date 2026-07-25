---
api_key_in:
- header
api_specs:
- filename: amazon-managed-blockchain-accessors-api-openapi.yml
  format: yaml
  label: Amazon Managed Blockchain Accessors API
  slug: amazon-managed-blockchain-accessors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/openapi/amazon-managed-blockchain-accessors-api-openapi.yml
- filename: amazon-managed-blockchain-invitations-api-openapi.yml
  format: yaml
  label: Amazon Managed Blockchain Invitations API
  slug: amazon-managed-blockchain-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/openapi/amazon-managed-blockchain-invitations-api-openapi.yml
- filename: amazon-managed-blockchain-networks-api-openapi.yml
  format: yaml
  label: Amazon Managed Blockchain Networks API
  slug: amazon-managed-blockchain-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/openapi/amazon-managed-blockchain-networks-api-openapi.yml
- filename: amazon-managed-blockchain-tags-api-openapi.yml
  format: yaml
  label: Amazon Managed Blockchain Tags API
  slug: amazon-managed-blockchain-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/openapi/amazon-managed-blockchain-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Managed Blockchain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Managed Blockchain secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-managed-blockchain-openapi-original.yaml
  type: apiKey
slug: amazon-managed-blockchain-authentication
source_filename: amazon-managed-blockchain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-managed-blockchain-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-managed-blockchain-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/authentication/amazon-managed-blockchain-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
---
