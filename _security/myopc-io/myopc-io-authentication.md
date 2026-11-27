---
anonymous_access: false
api_key_in: []
api_specs:
- filename: myopc-io-accounting-api-openapi.yml
  format: yaml
  label: OPC Suite Accounting API
  slug: myopc-io-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-accounting-api-openapi.yml
- filename: myopc-io-crm-api-openapi.yml
  format: yaml
  label: OPC Suite CRM API
  slug: myopc-io-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-crm-api-openapi.yml
- filename: myopc-io-hr-api-openapi.yml
  format: yaml
  label: OPC Suite HR API
  slug: myopc-io-hr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-hr-api-openapi.yml
- filename: myopc-io-inventory-api-openapi.yml
  format: yaml
  label: OPC Suite Inventory API
  slug: myopc-io-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-inventory-api-openapi.yml
- filename: myopc-io-sales-api-openapi.yml
  format: yaml
  label: OPC Suite Sales API
  slug: myopc-io-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-sales-api-openapi.yml
- filename: myopc-io-work-api-openapi.yml
  format: yaml
  label: OPC Suite Work API
  slug: myopc-io-work-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-work-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: OPC Suite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OPC Suite secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OPC Suite
provider_slug: myopc-io
scheme_count: 2
schemes:
- description: Personal access token (opc_pat_…) from /dashboard/settings/developer.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/myopc-io-openapi.json
  type: http
- description: OAuth 2.1 authorization code + PKCE.
  flows:
  - authorizationUrl: https://www.myopc.io/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://www.myopc.io/oauth/token
  name: oauth2
  sources:
  - openapi/myopc-io-openapi.json
  type: oauth2
slug: myopc-io-authentication
source_filename: myopc-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myopc-io-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token (opc_pat_…) from /dashboard/settings/developer.\n  sources:\n  - openapi/myopc-io-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.myopc.io/oauth/authorize\n    tokenUrl: https://www.myopc.io/oauth/token\n    scopes: 0\n  description: OAuth 2.1 authorization code + PKCE.\n  sources:\n  - openapi/myopc-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/myopc-io/authentication/myopc-io-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- ERP
- CRM
- Artificial Intelligence
- Business Management
- Software-as-a-Service
---
