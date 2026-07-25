---
api_key_in: []
api_specs:
- filename: polygon-id-agent-api-openapi.yml
  format: yaml
  label: Polygon ID Agent API
  slug: polygon-id-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-agent-api-openapi.yml
- filename: polygon-id-auth-api-openapi.yml
  format: yaml
  label: Polygon ID Auth API
  slug: polygon-id-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-auth-api-openapi.yml
- filename: polygon-id-config-api-openapi.yml
  format: yaml
  label: Polygon ID Config API
  slug: polygon-id-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-config-api-openapi.yml
- filename: polygon-id-connection-api-openapi.yml
  format: yaml
  label: Polygon ID Connection API
  slug: polygon-id-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-connection-api-openapi.yml
- filename: polygon-id-credentials-api-openapi.yml
  format: yaml
  label: Polygon ID Credentials API
  slug: polygon-id-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-credentials-api-openapi.yml
- filename: polygon-id-display-methods-api-openapi.yml
  format: yaml
  label: Polygon ID Display Methods API
  slug: polygon-id-display-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-display-methods-api-openapi.yml
- filename: polygon-id-identity-api-openapi.yml
  format: yaml
  label: Polygon ID Identity API
  slug: polygon-id-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-identity-api-openapi.yml
- filename: polygon-id-internal-api-openapi.yml
  format: yaml
  label: Polygon ID Internal API
  slug: polygon-id-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-internal-api-openapi.yml
- filename: polygon-id-key-management-api-openapi.yml
  format: yaml
  label: Polygon ID Key Management API
  slug: polygon-id-key-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-key-management-api-openapi.yml
- filename: polygon-id-links-api-openapi.yml
  format: yaml
  label: Polygon ID Links API
  slug: polygon-id-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-links-api-openapi.yml
- filename: polygon-id-payment-api-openapi.yml
  format: yaml
  label: Polygon ID Payment API
  slug: polygon-id-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-payment-api-openapi.yml
- filename: polygon-id-public-api-openapi.yml
  format: yaml
  label: Polygon ID Public API
  slug: polygon-id-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-public-api-openapi.yml
- filename: polygon-id-qr-store-api-openapi.yml
  format: yaml
  label: Polygon ID QR Store API
  slug: polygon-id-qr-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-qr-store-api-openapi.yml
- filename: polygon-id-schemas-api-openapi.yml
  format: yaml
  label: Polygon ID Schemas API
  slug: polygon-id-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/openapi/polygon-id-schemas-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Polygon Id Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polygon ID secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Polygon ID
provider_slug: polygon-id
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/issuer-node-api.yaml
  type: http
slug: polygon-id-authentication
source_filename: polygon-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/issuer-node-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/issuer-node-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon-id/refs/heads/main/authentication/polygon-id-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity
- Verifiable Credentials
- Zero-Knowledge Proofs
- Self-Sovereign Identity
- Decentralized Identity
- Blockchain
- Web3
- KYC
---
