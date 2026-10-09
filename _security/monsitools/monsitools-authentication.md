---
anonymous_access: false
api_key_in: []
api_specs:
- filename: monsitools-api-tools-json-api-openapi.yml
  format: yaml
  label: MonsiTools Api Tools.json API
  slug: monsitools-api-tools-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monsitools/refs/heads/main/openapi/monsitools-api-tools-json-api-openapi.yml
- filename: monsitools-calculate-api-openapi.yml
  format: yaml
  label: MonsiTools Calculate API
  slug: monsitools-calculate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monsitools/refs/heads/main/openapi/monsitools-calculate-api-openapi.yml
- filename: monsitools-keys-api-openapi.yml
  format: yaml
  label: MonsiTools Keys API
  slug: monsitools-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monsitools/refs/heads/main/openapi/monsitools-keys-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Monsitools Authentication
name_suffix: Authentication
oauth_flows: []
overview: MonsiTools secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MonsiTools
provider_slug: monsitools
scheme_count: 1
schemes:
- description: An API key (mt_live_...) for /api/calculate; a signed-in session token for /api/keys.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/monsitools-openapi.yml
  type: http
slug: monsitools-authentication
source_filename: monsitools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/monsitools-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An API key (mt_live_...) for /api/calculate; a signed-in session token for /api/keys.\n  sources:\n  - openapi/monsitools-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monsitools/refs/heads/main/authentication/monsitools-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Calculators
- Finance
- Workflows
- MCP
- Data Tools
---
