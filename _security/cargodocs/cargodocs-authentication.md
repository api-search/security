---
api_key_in: []
api_specs:
- filename: cargodocs-partner-openapi.yml
  format: yaml
  label: CargoDocs Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-partner-openapi.yml
- filename: cargodocs-issuer-openapi.yml
  format: yaml
  label: CargoDocs Issuer API
  slug: issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-issuer-openapi.yml
- filename: cargodocs-customer-openapi.yml
  format: yaml
  label: CargoDocs Customer Data/Docs API
  slug: customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-customer-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cargodocs Authentication
name_suffix: Authentication
oauth_flows: []
overview: CargoDocs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CargoDocs
provider_slug: cargodocs
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cargodocs-customer-openapi.yml
  - openapi/cargodocs-issuer-openapi.yml
  - openapi/cargodocs-partner-openapi.yml
  type: http
slug: cargodocs-authentication
source_filename: cargodocs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cargodocs-customer-openapi.yml, openapi/cargodocs-issuer-openapi.yml, openapi/cargodocs-partner-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cargodocs-customer-openapi.yml\n  - openapi/cargodocs-issuer-openapi.yml\n  - openapi/cargodocs-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/authentication/cargodocs-authentication.yml
summary_line: http · 1 scheme
tags:
- Bills of Lading
- Documentation
- eBoL
- EssDocs
- MLETR
- Shipping
- Supply Chain
- Trade
- Trade Finance
- Warehouse Warrants
---
