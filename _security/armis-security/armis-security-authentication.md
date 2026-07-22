---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Armis Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Armis Security secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Armis Security
provider_slug: armis-security
scheme_count: 2
schemes:
- flow: clientCredentials
  name: clientCredentials
  parameters:
  - client_id
  - client_secret
  - audience
  - vendor_id
  - scopes
  sources:
  - armis-sdk-python README
  - armis-knowledge-mcp README
  token_endpoint: /api/v1/auth/token
  type: oauth2
- in: header
  name: apiTokenLegacy
  note: Legacy Basic authentication (ARMIS_API_TOKEN + ARMIS_TENANT_ID), CLI-supported.
  scheme: basic
  sources:
  - armis-cli README
  type: apiKey
slug: armis-security-authentication
source_filename: armis-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://armis-python-sdk.readthedocs.io\ndocs: https://armis-python-sdk.readthedocs.io\nsummary:\n  types: [oauth2]\n  grant: client_credentials\n  token_format: jwt-bearer\n  multi_tenant: true\nnotes: >-\n  Armis uses a client-credentials model: a customer generates a Client ID and\n  Client Secret within their tenant, which the SDK/CLI/MCP clients exchange for a\n  short-lived JWT bearer token (POST /api/v1/auth/token). Requests are made\n  against the tenant host (audience, e.g. https://<tenant>.armis.com/). A\n  Vendor ID identifies the developer account/integration, and scopes may be\n  requested to bound access. A legacy Basic-auth model (API token + tenant id)\n  is still supported by the CLI.\nschemes:\n  - name: clientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: /api/v1/auth/token\n    parameters:\n      - client_id\n      - client_secret\n      - audience   # tenant URL, e.g. https://acme.armis.com/\n\
  \      - vendor_id\n      - scopes\n    sources: [armis-sdk-python README, armis-knowledge-mcp README]\n  - name: apiTokenLegacy\n    type: apiKey\n    in: header\n    scheme: basic\n    note: Legacy Basic authentication (ARMIS_API_TOKEN + ARMIS_TENANT_ID), CLI-supported.\n    sources: [armis-cli README]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armis-security/refs/heads/main/authentication/armis-security-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Asset Intelligence
- Cyber Exposure Management
- IoT Security
- OT Security
- Application Security
---
