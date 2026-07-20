---
api_key_in:
- header
api_specs:
- filename: galileo-technologies-openapi-original.json
  format: json
  label: Galileo API
  slug: galileo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-technologies/refs/heads/main/openapi/galileo-technologies-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Galileo Technologies Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Galileo Technologies secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Galileo Technologies
provider_slug: galileo-technologies
scheme_count: 4
schemes:
- in: header
  name: ClassicAPIKeyHeader
  parameter: Galileo-API-Key
  sources:
  - openapi/galileo-technologies-openapi-original.json
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: Splunk-AO-API-Key
  sources:
  - openapi/galileo-technologies-openapi-original.json
  type: apiKey
- flows:
  - flow: password
    scopes: 0
    tokenUrl: https://api.galileo.ai/login
  name: OAuth2PasswordBearer
  sources:
  - openapi/galileo-technologies-openapi-original.json
  type: oauth2
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/galileo-technologies-openapi-original.json
  type: http
slug: galileo-technologies-authentication
source_filename: galileo-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/galileo-technologies-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: ClassicAPIKeyHeader\n  type: apiKey\n  in: header\n  parameter: Galileo-API-Key\n  sources:\n  - openapi/galileo-technologies-openapi-original.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: Splunk-AO-API-Key\n  sources:\n  - openapi/galileo-technologies-openapi-original.json\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.galileo.ai/login\n    scopes: 0\n  sources:\n  - openapi/galileo-technologies-openapi-original.json\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/galileo-technologies-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galileo-technologies/refs/heads/main/authentication/galileo-technologies-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- AI Observability
- LLM Evaluation
- Generative AI
- Agents
- Monitoring
- Machine Learning
- Guardrails
- Developer Tools
---
