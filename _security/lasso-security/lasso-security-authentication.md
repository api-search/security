---
api_key_in:
- header
api_specs:
- filename: lasso-security-classify-api-openapi.yml
  format: yaml
  label: Lasso Security Classify API
  slug: lasso-security-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/openapi/lasso-security-classify-api-openapi.yml
- filename: lasso-security-masking-api-openapi.yml
  format: yaml
  label: Lasso Security Masking API
  slug: lasso-security-masking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/openapi/lasso-security-masking-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lasso Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lasso Security secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lasso Security
provider_slug: lasso-security
scheme_count: 1
schemes:
- description: Lasso API key issued from the Lasso dashboard (app.lasso.security).
  in: header
  name: LassoApiKey
  parameter: lasso-api-key
  sources:
  - openapi/lasso-security-openapi.yml
  type: apiKey
slug: lasso-security-authentication
source_filename: lasso-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lasso-security-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: LassoApiKey\n  type: apiKey\n  in: header\n  parameter: lasso-api-key\n  description: Lasso API key issued from the Lasso dashboard (app.lasso.security).\n  sources:\n  - openapi/lasso-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lasso-security/refs/heads/main/authentication/lasso-security-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- LLM
- GenAI Security
- Prompt Injection
- Guardrails
- MCP
---
