---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smartlead Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smartlead secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smartlead
provider_slug: smartlead-ai
scheme_count: 1
schemes:
- description: Smartlead API key passed as the `api_key` query parameter on every request.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/smartlead-ai-openapi.yml
  type: apiKey
slug: smartlead-ai-authentication
source_filename: smartlead-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartlead-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Smartlead API key passed as the `api_key` query parameter on every request.\n  sources:\n  - openapi/smartlead-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/authentication/smartlead-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cold Email
- Outbound
- Sales
- Deliverability
- Email Warmup
- Automation
- Sequences
---
