---
api_key_in:
- header
api_specs:
- filename: vectranetworks-rux-v3.3-openapi.yml
  format: yaml
  label: Vectra AI Platform API (RUX)
  slug: vectra-ai-platform-api-rux
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-rux-v3.3-openapi.yml
- filename: vectranetworks-detect-v2.3-openapi.yml
  format: yaml
  label: Vectra Detect API
  slug: vectra-detect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-detect-v2.3-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vectranetworks Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Vectra AI secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Vectra AI
provider_slug: vectranetworks
scheme_count: 2
schemes:
- in: header
  name: VectraToken
  parameter: authorization
  sources:
  - openapi/vectranetworks-detect-v2.3-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{vectra_portal_url}/oauth2/token
  name: oauth2
  sources:
  - openapi/vectranetworks-rux-v3.3-openapi.yml
  type: oauth2
slug: vectranetworks-authentication
source_filename: vectranetworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vectranetworks-detect-v2.3-openapi.yml, openapi/vectranetworks-rux-v3.3-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: VectraToken\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/vectranetworks-detect-v2.3-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{vectra_portal_url}/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/vectranetworks-rux-v3.3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/authentication/vectranetworks-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Cybersecurity
- Network Detection and Response
- Threat Detection
- Security Operations
- Artificial Intelligence
- SIEM
---
