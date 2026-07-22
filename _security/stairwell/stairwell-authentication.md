---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Stairwell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stairwell secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stairwell
provider_slug: stairwell
scheme_count: 1
schemes:
- description: Stairwell API and CLI tokens are long-lived opaque bearer tokens minted in the web app under Settings > Auth tokens (Organization), token type "API/CLI". The token is shown only once at creation. All requests to https://app.stairwell.com/v1 carry it in the Authorization header.
  format: 'Authorization: Bearer YOUR_API_TOKEN'
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.stairwell.com/docs/api-quickstart.md
  type: http
slug: stairwell-authentication
source_filename: stairwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.stairwell.com/docs/api-quickstart.md\ndocs: https://docs.stairwell.com/docs/api-token-scope.md\nsummary:\n  types: [http]\n  scheme: bearer\n  token_style: opaque-api-token\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: 'Authorization: Bearer YOUR_API_TOKEN'\n    sources: [https://docs.stairwell.com/docs/api-quickstart.md]\n    description: >-\n      Stairwell API and CLI tokens are long-lived opaque bearer tokens minted in\n      the web app under Settings > Auth tokens (Organization), token type\n      \"API/CLI\". The token is shown only once at creation. All requests to\n      https://app.stairwell.com/v1 carry it in the Authorization header.\naccess_model:\n  description: >-\n    A token grants access corresponding to its creation level. For MSSP\n    parent/child (multi-tenant) relationships, a token created\
  \ at the parent\n    level is granted access to all child environments and shared environments\n    including global objects. There are no named OAuth scopes; access is scoped\n    by environment hierarchy and the creating principal's role.\n  source: https://docs.stairwell.com/docs/api-token-scope.md\nguidance:\n  - Treat the API token like a password; do not commit tokens to source control.\n  - Revoke compromised tokens immediately from Settings > Auth tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stairwell/refs/heads/main/authentication/stairwell-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Threat Intelligence
- Malware Analysis
- Cybersecurity
- Threat Detection
- YARA
- Incident Response
---
