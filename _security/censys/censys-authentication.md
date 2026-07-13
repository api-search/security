---
api_key_in: []
api_specs:
- filename: censys-platform-openapi.yml
  format: yaml
  label: Censys Platform API
  slug: censys-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-platform-openapi.yml
- filename: censys-asset-graph-openapi.yml
  format: yaml
  label: Censys Asset Graph API
  slug: censys-asset-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-asset-graph-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Censys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Censys secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Censys
provider_slug: censys
scheme_count: 1
schemes:
- description: Your Censys personal access token.
  name: PersonalAccessToken
  scheme: bearer
  sources:
  - openapi/censys-asset-graph-openapi.yml
  - openapi/censys-platform-openapi.yml
  type: http
slug: censys-authentication
source_filename: censys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/censys-asset-graph-openapi.yml, openapi/censys-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  description: Your Censys personal access token.\n  sources:\n  - openapi/censys-asset-graph-openapi.yml\n  - openapi/censys-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/authentication/censys-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Internet Intelligence
- Attack Surface Management
- Threat Hunting
- Cyber Threat Intelligence
- OSINT
- Internet Scanning
- Certificates
- Asset Discovery
---
