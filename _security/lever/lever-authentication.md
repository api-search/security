---
api_key_in: []
api_specs:
- filename: lever-openapi.yml
  format: yaml
  label: Lever Opportunities API
  slug: lever-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever/refs/heads/main/openapi/lever-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lever Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lever secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lever
provider_slug: lever
scheme_count: 2
schemes:
- description: API key supplied as the basic auth username with empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/lever-openapi.yml
  type: http
- description: OAuth 2.0 bearer access token (Lever Partner OAuth apps).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lever-openapi.yml
  type: http
slug: lever-authentication
source_filename: lever-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lever-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API key supplied as the basic auth username with empty password.\n  sources:\n  - openapi/lever-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer access token (Lever Partner OAuth apps).\n  sources:\n  - openapi/lever-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lever/refs/heads/main/authentication/lever-authentication.yml
summary_line: http · 2 schemes
tags:
- HR
- ATS
- Recruiting
- Talent Acquisition
- SaaS
---
