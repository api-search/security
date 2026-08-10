---
api_key_in: []
api_specs:
- filename: digital-asset-common-api-openapi.yml
  format: yaml
  label: Digital Asset Common API
  slug: digital-asset-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/openapi/digital-asset-common-api-openapi.yml
- filename: digital-asset-operator-api-openapi.yml
  format: yaml
  label: Digital Asset Operator API
  slug: digital-asset-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/openapi/digital-asset-operator-api-openapi.yml
- filename: digital-asset-public-api-openapi.yml
  format: yaml
  label: Digital Asset Public API
  slug: digital-asset-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/openapi/digital-asset-public-api-openapi.yml
- filename: digital-asset-registry-api-openapi.yml
  format: yaml
  label: Digital Asset Registry API
  slug: digital-asset-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/openapi/digital-asset-registry-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Digital Asset Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digital Asset secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Digital Asset
provider_slug: digital-asset
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/digital-asset-utilities-openapi.yml
  - openapi/digital-asset-utilities-runtime-openapi.yml
  type: http
slug: digital-asset-authentication
source_filename: digital-asset-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/digital-asset-utilities-openapi.yml, openapi/digital-asset-utilities-runtime-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/digital-asset-utilities-openapi.yml\n  - openapi/digital-asset-utilities-runtime-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/authentication/digital-asset-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Tokenization
- Digital Assets
- Financial Services
- Distributed Ledger
- Smart Contracts
- Capital Markets
- Canton Network
- Daml
- Stablecoins
---
