---
api_key_in:
- header
api_specs:
- filename: eigenpal-openapi-original.json
  format: json
  label: Eigenpal API
  slug: eigenpal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eigenpal/refs/heads/main/openapi/eigenpal-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Eigenpal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eigenpal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eigenpal
provider_slug: eigenpal
scheme_count: 1
schemes:
- description: 'API key issued from the dashboard under Settings → API Keys. Pass as `Authorization: Bearer <key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eigenpal-openapi-original.json
  type: http
slug: eigenpal-authentication
source_filename: eigenpal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/eigenpal-openapi-original.json\ndocs: https://docs.eigenpal.com/api-reference\nsummary:\n  types:\n  - http\n  scheme: bearer-api-key\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued from the dashboard under Settings → API Keys. Pass as `Authorization: Bearer <key>`.'\n  sources:\n  - openapi/eigenpal-openapi-original.json\nnotes:\n  key_issuance: Dashboard → Settings → API Keys (one key maps to one tenant/organization).\n  cli_login: '`eigenpal auth login` opens a browser to create an API key and stores it in ~/.config/eigenpal/credentials.json as a named profile.'\n  identity_endpoint: 'GET /api/v1/auth/check returns the tenant, user, API key, and scope for the current key.'\n  scopes: API keys carry a scope; a 403 is returned when the key lacks the scope required by an operation (key-level scopes, not OAuth scopes).\n  self_hosted:\
  \ SDKs and CLI accept a custom base URL (baseUrl / base_url / EIGENPAL server profile) to target self-hosted deployments.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eigenpal/refs/heads/main/authentication/eigenpal-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Document Processing
- Artificial Intelligence
- Workflow Automation
- Machine Learning
- Data Extraction
- OCR
- Developer Tools
- Enterprise
---
