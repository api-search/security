---
api_key_in:
- header
api_specs:
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Tokens API
  slug: basis-theory-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Tokenize / Detokenize API
  slug: basis-theory-tokenize-detokenize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Applications API
  slug: basis-theory-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Proxy API
  slug: basis-theory-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Reactors API
  slug: basis-theory-reactors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory 3D Secure API
  slug: basis-theory-3ds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Tenants API
  slug: basis-theory-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
- filename: basis-theory-openapi.yml
  format: yaml
  label: Basis Theory Webhooks API
  slug: basis-theory-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/openapi/basis-theory-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Basis Theory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basis Theory secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basis Theory
provider_slug: basis-theory
scheme_count: 1
schemes:
- description: Authenticate every request with a Basis Theory Application key supplied in the BT-API-KEY request header.
  in: header
  name: ApiKey
  parameter: BT-API-KEY
  sources:
  - openapi/basis-theory-openapi.yml
  type: apiKey
slug: basis-theory-authentication
source_filename: basis-theory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basis-theory-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: BT-API-KEY\n  description: Authenticate every request with a Basis Theory Application key supplied in the\n    BT-API-KEY request header.\n  sources:\n  - openapi/basis-theory-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basis-theory/refs/heads/main/authentication/basis-theory-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Tokenization
- Data Vault
- PCI Compliance
- Payments
- Security
---
