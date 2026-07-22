---
api_key_in: []
api_specs:
- filename: xentral-api-openapi-original.json
  format: json
  label: Xentral API
  slug: xentral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/openapi/xentral-api-openapi-original.json
- filename: xentral-documents-api-openapi-original.json
  format: json
  label: Xentral Business Documents API v3
  slug: xentral-business-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/openapi/xentral-documents-api-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Xentral Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xentral secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Xentral
provider_slug: xentral
scheme_count: 1
schemes:
- description: Bearer token obtained in POST /tokens endpoint or pregenerated in the system.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/xentral-api-openapi-original.json
  - openapi/xentral-documents-api-openapi-original.json
  type: http
slug: xentral-authentication
source_filename: xentral-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/xentral-api-openapi-original.json, openapi/xentral-documents-api-openapi-original.json\ndocs: https://developer.xentral.com/reference/authentication\nsummary:\n  types:\n  - http\n  scheme: bearer (Personal Access Token)\n  scopes: v3 Business Documents endpoints require per-endpoint token scopes (resource:action)\nnotes: Authentication for all Xentral APIs (current API, legacy REST API, legacy Standard\n  API) is via Personal Access Tokens (PATs) created under Administration > Account settings\n  > Developer Settings > Personal Access Tokens (admin rights required). Tokens are shown\n  once at creation, have unlimited permissions and no expiration date, and can be revoked\n  by deletion at any time. Some legacy /shopimport/* and /v1/reports endpoints are not\n  accessible with PATs. More granular token access control is documented as a planned\n  enhancement.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n\
  \  description: Bearer token obtained in POST /tokens endpoint or pregenerated in the system.\n  sources:\n  - openapi/xentral-api-openapi-original.json\n  - openapi/xentral-documents-api-openapi-original.json\nscopes_artifact: scopes/xentral-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/authentication/xentral-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- ERP
- eCommerce
- Fulfillment
- Warehousing
- Invoicing
- Accounting
- Orders
- Products
- Germany
---
