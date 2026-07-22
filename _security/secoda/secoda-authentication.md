---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Secoda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Secoda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Secoda
provider_slug: secoda
scheme_count: 1
schemes:
- description: 'Secoda API requests authenticate with a workspace API key passed in the Authorization header as a Bearer token (Authorization: Bearer <API_KEY>). The key is generated from workspace Settings > API and grants the same workspace access as the user who created it. No OAuth or scopes are documented; access is governed by the creating user''s role and permissions.'
  format: Bearer <API_KEY>
  location: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - docs.secoda.co/api/authentication
  token_url: https://app.secoda.co/settings/api
  type: http
slug: secoda-authentication
source_filename: secoda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.secoda.co/api/authentication\ndocs: https://docs.secoda.co/api/authentication\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Secoda API requests authenticate with a workspace API key passed in the\n      Authorization header as a Bearer token (Authorization: Bearer <API_KEY>).\n      The key is generated from workspace Settings > API and grants the same\n      workspace access as the user who created it. No OAuth or scopes are\n      documented; access is governed by the creating user's role and permissions.\n    location: header\n    parameter: Authorization\n    format: 'Bearer <API_KEY>'\n    token_url: https://app.secoda.co/settings/api\n    sources: [docs.secoda.co/api/authentication]\nnotes:\n  - Regional base hosts each require a key from that region's workspace.\n\
  \  - MCP server passes the same key as an API_TOKEN environment variable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secoda/refs/heads/main/authentication/secoda-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Data Catalog
- Data Governance
- Metadata
- Data Lineage
- Data Quality
- Data Discovery
- Observability
- AI Agents
---
