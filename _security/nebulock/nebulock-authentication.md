---
api_key_in:
- header
api_specs:
- filename: nebulock-openapi.yml
  format: yaml
  label: Nebulock Public API
  slug: nebulock-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nebulock/refs/heads/main/openapi/nebulock-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nebulock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nebulock secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nebulock
provider_slug: nebulock
scheme_count: 2
schemes:
- in: header
  name: ApiKeyId
  parameter: X-API-Key-ID
  sources:
  - openapi/nebulock-openapi.yml
  type: apiKey
- in: header
  name: ApiKeySecret
  parameter: X-API-Key-Secret
  sources:
  - openapi/nebulock-openapi.yml
  type: apiKey
slug: nebulock-authentication
source_filename: nebulock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nebulock-openapi.yml\ndocs: https://docs.nebulock.io/reference/getting-started-with-the-nebulock-findings-api\nnotes: >-\n  The Nebulock public API is available only to active Nebulock customers.\n  API keys are issued and managed by organization administrators in the Nebulock\n  platform (see https://docs.nebulock.io/docs/create-an-api-key). Every request\n  must carry two headers: X-API-Key-ID and X-API-Key-Secret. Portal/user access\n  to the Nebulock platform itself is via SAML SSO (Okta or Microsoft Entra).\n  Rate limit: 60 requests per minute.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  portal_sso:\n  - SAML (Okta)\n  - SAML (Microsoft Entra)\n  rate_limit: 60/min\nschemes:\n- name: ApiKeyId\n  type: apiKey\n  in: header\n  parameter: X-API-Key-ID\n  sources:\n  - openapi/nebulock-openapi.yml\n- name: ApiKeySecret\n  type: apiKey\n  in: header\n  parameter: X-API-Key-Secret\n  sources:\n  -\
  \ openapi/nebulock-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nebulock/refs/heads/main/authentication/nebulock-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Security
- Threat Hunting
- Threat Detection
- Security Operations
- Detection Engineering
- AI Agents
- SIEM
---
