---
api_key_in:
- header
api_specs:
- filename: wallarm-applications-api-openapi.yml
  format: yaml
  label: Wallarm Applications API
  slug: wallarm-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-applications-api-openapi.yml
- filename: wallarm-attacks-api-openapi.yml
  format: yaml
  label: Wallarm Attacks API
  slug: wallarm-attacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-attacks-api-openapi.yml
- filename: wallarm-integrations-api-openapi.yml
  format: yaml
  label: Wallarm Integrations API
  slug: wallarm-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-integrations-api-openapi.yml
- filename: wallarm-ip-lists-api-openapi.yml
  format: yaml
  label: Wallarm IP Lists API
  slug: wallarm-ip-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-ip-lists-api-openapi.yml
- filename: wallarm-nodes-api-openapi.yml
  format: yaml
  label: Wallarm Nodes API
  slug: wallarm-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-nodes-api-openapi.yml
- filename: wallarm-rules-api-openapi.yml
  format: yaml
  label: Wallarm Rules API
  slug: wallarm-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-rules-api-openapi.yml
- filename: wallarm-triggers-api-openapi.yml
  format: yaml
  label: Wallarm Triggers API
  slug: wallarm-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-triggers-api-openapi.yml
- filename: wallarm-user-api-openapi.yml
  format: yaml
  label: Wallarm User API
  slug: wallarm-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-user-api-openapi.yml
- filename: wallarm-vulnerabilities-api-openapi.yml
  format: yaml
  label: Wallarm Vulnerabilities API
  slug: wallarm-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-vulnerabilities-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wallarm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wallarm secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wallarm
provider_slug: wallarm
scheme_count: 1
schemes:
- description: API token obtained from Wallarm Console under Settings → API Tokens.
  in: header
  name: ApiTokenAuth
  parameter: X-WallarmApi-Token
  sources:
  - openapi/wallarm-openapi.yml
  type: apiKey
slug: wallarm-authentication
source_filename: wallarm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wallarm-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-WallarmApi-Token\n  description: API token obtained from Wallarm Console under Settings → API Tokens.\n  sources:\n  - openapi/wallarm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/authentication/wallarm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Security
- Security Testing
- WAF
- Cybersecurity
---
