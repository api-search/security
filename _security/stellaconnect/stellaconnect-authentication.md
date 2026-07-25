---
api_key_in:
- header
api_specs:
- filename: stellaconnect-coaching-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Coaching API
  slug: stellaconnect-coaching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-coaching-api-openapi.yml
- filename: stellaconnect-data-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Data API
  slug: stellaconnect-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-data-api-openapi.yml
- filename: stellaconnect-employees-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Employees API
  slug: stellaconnect-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-employees-api-openapi.yml
- filename: stellaconnect-qa-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Qa API
  slug: stellaconnect-qa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-qa-api-openapi.yml
- filename: stellaconnect-recoveries-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Recoveries API
  slug: stellaconnect-recoveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-recoveries-api-openapi.yml
- filename: stellaconnect-requests-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Requests API
  slug: stellaconnect-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-requests-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Stellaconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stella Connect (Medallia Agent Connect) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stella Connect (Medallia Agent Connect)
provider_slug: stellaconnect
scheme_count: 2
schemes:
- description: Agent Connect API key (test or production), issued per client on the Integrations settings page.
  in: header
  name: ApiKeyInHeader
  parameter: x-api-key
  sources:
  - openapi/stellaconnect-data-return-openapi-original.yml
  - openapi/stellaconnect-requests-openapi-original.yml
  - openapi/stellaconnect-user-management-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT signed with the company API secret using HMAC SHA256, containing a valid iat claim, provided via the Authorization header. Required for User Management and Data Return endpoints, not for Feedback and service recovery requests.
  name: JwtAuth
  scheme: bearer
  sources:
  - openapi/stellaconnect-data-return-openapi-original.yml
  - openapi/stellaconnect-user-management-openapi-original.yml
  type: http
slug: stellaconnect-authentication
source_filename: stellaconnect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.medallia.com/en/agent-connect/api/authentication\nsource: openapi/stellaconnect-data-return-openapi-original.yml, openapi/stellaconnect-requests-openapi-original.yml,\n  openapi/stellaconnect-user-management-openapi-original.yml\nnotes: >-\n  Each Agent Connect client is issued two API keys — one test key and one production key — generated\n  on the Integrations settings page (Settings > Integrations) inside Agent Connect. All requests must\n  be made over HTTPS. The Requests API (/v1/requests, /v1/recoveries) authenticates with the x-api-key\n  header alone. The Data Return and User Management APIs additionally require a JSON Web Token, signed\n  with the company's API secret using HMAC SHA256 and containing a valid iat claim, sent in the\n  Authorization header alongside the x-api-key header.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyInHeader\n  type: apiKey\n\
  \  in: header\n  parameter: x-api-key\n  description: Agent Connect API key (test or production), issued per client on the Integrations settings\n    page.\n  sources:\n  - openapi/stellaconnect-data-return-openapi-original.yml\n  - openapi/stellaconnect-requests-openapi-original.yml\n  - openapi/stellaconnect-user-management-openapi-original.yml\n- name: JwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT signed with the company API secret using HMAC SHA256, containing a valid iat claim,\n    provided via the Authorization header. Required for User Management and Data Return endpoints, not\n    for Feedback and service recovery requests.\n  sources:\n  - openapi/stellaconnect-data-return-openapi-original.yml\n  - openapi/stellaconnect-user-management-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/authentication/stellaconnect-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Customer Service
- Customer Feedback
- Quality Assurance
- Coaching
- Contact Centers
- Surveys
- Customer Experience
- SaaS
---
