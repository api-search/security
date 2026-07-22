---
api_key_in: []
api_specs:
- filename: rasgo-openapi.yml
  format: yaml
  label: Rasgo API
  slug: rasgo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasgo/refs/heads/main/openapi/rasgo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rasgo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rasgo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rasgo
provider_slug: rasgo
scheme_count: 1
schemes:
- description: Personal Rasgo API key sent as an HTTP Bearer token in the Authorization header. Enterprise users copy their key from the Rasgo WebApp (User Profile > API Key). Keys are unique and personal and grant access to the caller's data; Rasgo warns against sharing or committing them.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rasgo-openapi.yml
  type: http
slug: rasgo-authentication
source_filename: rasgo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.rasgoml.com/rasgo-docs/api.md\ndocs: https://docs.rasgoml.com/rasgo-docs/api.md\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  availability: Enterprise plans and above\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Personal Rasgo API key sent as an HTTP Bearer token in the Authorization header.\n      Enterprise users copy their key from the Rasgo WebApp (User Profile > API Key). Keys\n      are unique and personal and grant access to the caller's data; Rasgo warns against\n      sharing or committing them.\n    sources: [openapi/rasgo-openapi.yml]\nnotes:\n  - Requests also send a `Rasgo-Client: API` header per the documented code samples.\n  - No OAuth2 / OIDC scopes are documented; access is a single personal API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rasgo/refs/heads/main/authentication/rasgo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Warehouse
- Analytics
- Artificial Intelligence
- Natural Language
- Snowflake
- BigQuery
- Business Intelligence
- Metadata
- SQL
---
