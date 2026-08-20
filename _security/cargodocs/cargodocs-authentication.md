---
api_key_in: []
api_specs:
- filename: cargodocs-common-api-openapi.yml
  format: yaml
  label: CargoDocs Common API
  slug: cargodocs-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-common-api-openapi.yml
- filename: cargodocs-documents-api-openapi.yml
  format: yaml
  label: CargoDocs Documents API
  slug: cargodocs-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-documents-api-openapi.yml
- filename: cargodocs-exchange-api-openapi.yml
  format: yaml
  label: CargoDocs Exchange API
  slug: cargodocs-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-exchange-api-openapi.yml
- filename: cargodocs-import-api-openapi.yml
  format: yaml
  label: CargoDocs Import API
  slug: cargodocs-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-import-api-openapi.yml
- filename: cargodocs-issuance-api-openapi.yml
  format: yaml
  label: CargoDocs Issuance API
  slug: cargodocs-issuance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-issuance-api-openapi.yml
- filename: cargodocs-surrender-api-openapi.yml
  format: yaml
  label: CargoDocs Surrender API
  slug: cargodocs-surrender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-surrender-api-openapi.yml
- filename: cargodocs-transactions-api-openapi.yml
  format: yaml
  label: CargoDocs Transactions API
  slug: cargodocs-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-transactions-api-openapi.yml
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
- eBOL
- EssDocs
- MLETR
- Shipping
- Supply Chain
- Trade
- Trade Finance
- Warehouse Warrants
---
