---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Forex Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: FOREX.com secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FOREX.com
provider_slug: forex-com
scheme_count: 2
schemes:
- description: Session ID obtained from POST /session
  in: header
  name: SessionAuth
  parameter: Session
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: FOREX.com account username
  in: header
  name: UserNameAuth
  parameter: UserName
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: forex-com-authentication
source_filename: forex-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SessionAuth\n  type: apiKey\n  in: header\n  parameter: Session\n  description: Session ID obtained from POST /session\n  sources:\n  - openapi/openapi.yml\n- name: UserNameAuth\n  type: apiKey\n  in: header\n  parameter: UserName\n  description: FOREX.com account username\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forex-com/refs/heads/main/authentication/forex-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Forex
- FX Trading
- CFD Trading
- Algorithmic Trading
- Financial Services
- Trading APIs
- Currency Exchange
---
