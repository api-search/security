---
api_key_in:
- header
api_specs:
- filename: instabase-aihub-openapi.yaml
  format: yaml
  label: Instabase AI Hub API
  slug: instabase-ai-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instabase/refs/heads/main/openapi/instabase-aihub-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Instabase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instabase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Instabase
provider_slug: instabase
scheme_count: 1
schemes:
- bearerFormat: auth-scheme
  description: 'Bearer HTTP authentication. Users create AI Hub API tokens under Settings > APIs > AI Hub tokens (named, with an expiration); the token value is shown once. Passed as `Authorization: Bearer ${API_TOKEN}`. A token grants the same access/permissions as its creating user or service account.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/instabase-aihub-openapi.yaml
  type: http
slug: instabase-authentication
source_filename: instabase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/instabase-aihub-openapi.yaml\ndocs: https://docs.instabase.com/api-sdk/authorization.md\nsummary:\n  types:\n  - http\n  api_key_in: [header]\n  bearer: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: auth-scheme\n  description: >-\n    Bearer HTTP authentication. Users create AI Hub API tokens under\n    Settings > APIs > AI Hub tokens (named, with an expiration); the token\n    value is shown once. Passed as `Authorization: Bearer ${API_TOKEN}`.\n    A token grants the same access/permissions as its creating user or\n    service account.\n  sources:\n  - openapi/instabase-aihub-openapi.yaml\ncontext_header:\n  name: IB-Context\n  required: true\n  values: >-\n    Organization ID (organization and service accounts) or User ID\n    (community accounts, deprecated). Identifies the request context and\n    where files are accessed.\nexternal_oauth:\n  supported: true\n  tier: enterprise\n\
  \  note: >-\n    External IdP/OIDC tokens can be used for API access\n    (ENABLE_EXTERNAL_IDP_TOKENS_FOR_API_ACCESS); if the token carries a\n    valid scope claim, AI Hub authorizes based on the roles in that scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instabase/refs/heads/main/authentication/instabase-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Intelligent Document Processing
- Document AI
- Artificial Intelligence
- Machine Learning
- Automation
- Data Extraction
- LLM
- Financial Services
- Insurance
---
