---
api_key_in:
- header
api_specs:
- filename: emarsys-openapi.yml
  format: yaml
  label: SAP Emarsys Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emarsys/refs/heads/main/openapi/emarsys-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Emarsys Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP Emarsys secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP Emarsys
provider_slug: emarsys
scheme_count: 2
schemes:
- description: Legacy WSSE authentication header (being deprecated).
  in: header
  name: WSSE
  parameter: X-WSSE
  sources:
  - openapi/emarsys-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.emarsys.net/api/v3/auth/token
  name: OAuth2
  sources:
  - openapi/emarsys-openapi.yml
  type: oauth2
slug: emarsys-authentication
source_filename: emarsys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/emarsys-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: WSSE\n  type: apiKey\n  in: header\n  parameter: X-WSSE\n  description: Legacy WSSE authentication header (being deprecated).\n  sources:\n  - openapi/emarsys-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.emarsys.net/api/v3/auth/token\n    scopes: 0\n  sources:\n  - openapi/emarsys-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emarsys/refs/heads/main/authentication/emarsys-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Marketing Automation
- Customer Engagement
- Email Marketing
- Omnichannel
- Customer Data Platform
- SAP
---
