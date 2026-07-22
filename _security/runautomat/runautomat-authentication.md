---
api_key_in: []
api_specs:
- filename: runautomat-extract-openapi.json
  format: json
  label: Automat Document Extraction API
  slug: automat-document-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runautomat/refs/heads/main/openapi/runautomat-extract-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Runautomat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runautomat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Runautomat
provider_slug: runautomat
scheme_count: 1
schemes:
- format: Bearer ak_<api_key>
  header: Authorization
  in: header
  name: BearerAuthScheme
  scheme: bearer
  sources:
  - openapi/runautomat-extract-openapi.json
  type: http
slug: runautomat-authentication
source_filename: runautomat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/runautomat-extract-openapi.json\ndocs: https://docs.runautomat.com/guides/getting-started/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_prefix: ak_\nnotes: >-\n  All API requests to Automat require an API key passed as an HTTP Bearer token\n  in the Authorization header (\"Authorization: Bearer ak_...\"). API keys are\n  scoped to the organization and grant access to all extractors within it. Keys\n  are created in the Automat dashboard (Settings -> API Keys), shown once, and\n  can be revoked independently. There is no OAuth/OIDC surface on the public\n  Extract API.\nschemes:\n- name: BearerAuthScheme\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer ak_<api_key>'\n  sources:\n  - openapi/runautomat-extract-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runautomat/refs/heads/main/authentication/runautomat-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automation
- Robotic Process Automation
- Document Processing
- Artificial Intelligence
- Machine Learning
- Data Extraction
- iPaaS
- Agents
---
