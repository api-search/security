---
api_key_in: []
api_specs:
- filename: vicai-openapi-original.json
  format: json
  label: Vic.ai API
  slug: vicai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vicai/refs/heads/main/openapi/vicai-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Vicai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vic.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vic.ai
provider_slug: vicai
scheme_count: 1
schemes:
- bearer_format: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/vicai-openapi-original.json
  type: http
slug: vicai-authentication
source_filename: vicai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.vic.ai (Authentication) + openapi/vicai-openapi-original.json\ndocs: https://docs.vic.ai\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  model: client-credentials -> Bearer JWT\nflow:\n  token_endpoint: POST /v0/token\n  request_body: '{ \"client_id\": \"...\", \"client_secret\": \"...\" }'\n  response: '{ \"access_token\": \"<JWT>\", \"token_type\": \"Bearer\", \"expires_in\": 3600 }'\n  usage: 'Authorization: Bearer <access_token>'\n  ttl_seconds: 3600\n  credentials_source: Issued securely by a Vic.ai representative on request (no self-service key provisioning).\n  notes:\n  - Access tokens are JWTs and may exceed 530 characters; storage must not impose a character limit.\n  - Credentials are the keys to the ERP integration and must be kept secret.\n  - Rate limiting and most authorization is scoped per OAuth client id.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearer_format:\
  \ JWT\n  sources:\n  - openapi/vicai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vicai/refs/heads/main/authentication/vicai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Accounts Payable
- Invoicing
- Payments
- ERP Integration
- AI
- Finance Automation
- Webhooks
---
