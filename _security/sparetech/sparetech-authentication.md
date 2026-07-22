---
api_key_in: []
api_specs:
- filename: sparetech-sync-v1-openapi.json
  format: json
  label: Sparetech Sync API v1
  slug: sparetech-sync-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparetech/refs/heads/main/openapi/sparetech-sync-v1-openapi.json
- filename: sparetech-sync-v2-openapi.json
  format: json
  label: Sparetech Sync API v2 (SAP)
  slug: sparetech-sync-api-v2-sap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparetech/refs/heads/main/openapi/sparetech-sync-v2-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sparetech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sparetech secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sparetech
provider_slug: sparetech
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: This API uses JWT for authorization. SPARETECH will provide your client credentials, that are specific to each organisation and integration environment. See the Authentication section of this documentation for details on how to obtain a token.
  name: Token
  scheme: bearer
  sources:
  - openapi/sparetech-sync-v1-openapi.json
  - openapi/sparetech-sync-v2-openapi.json
  type: http
- name: ClientCredentials
  scheme: basic
  sources:
  - openapi/sparetech-sync-v1-openapi.json
  - openapi/sparetech-sync-v2-openapi.json
  type: http
slug: sparetech-authentication
source_filename: sparetech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sparetech-sync-v1-openapi.json, openapi/sparetech-sync-v2-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: This API uses JWT for authorization. SPARETECH will provide your client credentials,\n    that are specific to each organisation and integration environment. See the Authentication\n    section of this documentation for details on how to obtain a token.\n  sources:\n  - openapi/sparetech-sync-v1-openapi.json\n  - openapi/sparetech-sync-v2-openapi.json\n- name: ClientCredentials\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sparetech-sync-v1-openapi.json\n  - openapi/sparetech-sync-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparetech/refs/heads/main/authentication/sparetech-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Manufacturing
- Spare Parts
- MRO
- Maintenance
- Procurement
- Inventory Optimization
- ERP Integration
- SAP
- Master Data Management
---
