---
anonymous_access: true
api_key_in: []
api_specs:
- filename: codefmt-dev-ask-api-openapi.yml
  format: yaml
  label: codefmt Ask API
  slug: codefmt-dev-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codefmt-dev/openapi/codefmt-dev-ask-api-openapi.yml
- filename: codefmt-dev-format-api-openapi.yml
  format: yaml
  label: codefmt Format API
  slug: codefmt-dev-format-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codefmt-dev/openapi/codefmt-dev-format-api-openapi.yml
- filename: codefmt-dev-health-api-openapi.yml
  format: yaml
  label: codefmt Health API
  slug: codefmt-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codefmt-dev/openapi/codefmt-dev-health-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: codefmt Authentication
name_suffix: Authentication
oauth_flows: []
overview: codefmt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: codefmt
provider_slug: codefmt-dev
scheme_count: 1
schemes:
- description: codefmt requires **no authentication**. Every public endpoint is open and rate-limited per IP. There are no user accounts, API keys, bearer tokens, OAuth/OIDC, or agent registration of any kind. All access is anonymous.
  evidence: https://codefmt.dev/auth.md
  type: none
slug: codefmt-dev-authentication
source_filename: codefmt-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codefmt.dev/auth.md\ndocs: https://codefmt.dev/auth.md\nsummary: codefmt requires no authentication. Every public endpoint (format API, MCP, A2A, /ask) is anonymous and rate-limited per IP; the OpenAPI declares no securitySchemes.\nschemes:\n- type: none\n  description: \"codefmt requires **no authentication**. Every public endpoint is open and rate-limited per IP. There are no user accounts, API keys, bearer tokens, OAuth/OIDC, or agent registration of any kind. All access is anonymous.\"\n  evidence: https://codefmt.dev/auth.md\n"
source_yaml_url: https://artifacts.apis.io/codefmt-dev/authentication/codefmt-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Code Formatting
- Linting
- HubL
- HubSpot
- Zapier
- n8n
- Automation
- Developer Tools
- MCP
---
