---
api_key_in: []
api_specs:
- filename: evrim-openapi-original.yml
  format: yaml
  label: Evrim API
  slug: evrim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Evrim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evrim secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Evrim
provider_slug: evrim
scheme_count: 1
schemes:
- applied_to_all_operations: true
  description: Django Knox API token presented as a Bearer credential in the Authorization header. Token supplied to the SDK via EVRIM_API_TOKEN.
  evidence:
  - https://github.com/evrimai/python-client/blob/HEAD/README.md
  name: knoxApiToken
  scheme: bearer
  sources:
  - openapi/evrim-openapi-original.yml
  type: http
slug: evrim-authentication
source_filename: evrim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/evrim-openapi-original.yml\ndocs: https://docs.evrim.ai\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Evrim authenticates every operation with a single Knox-issued API token\n  presented as an HTTP Bearer credential (Authorization: Bearer <token>). The\n  official Python SDK reads the token from the EVRIM_API_TOKEN environment\n  variable (or an `api_token` client keyword). All 91 operations apply the\n  knoxApiToken scheme; there is no OAuth2/OIDC and no API-key query or header\n  parameter.\nschemes:\n- name: knoxApiToken\n  type: http\n  scheme: bearer\n  description: >-\n    Django Knox API token presented as a Bearer credential in the Authorization\n    header. Token supplied to the SDK via EVRIM_API_TOKEN.\n  applied_to_all_operations: true\n  sources:\n  - openapi/evrim-openapi-original.yml\n  evidence:\n  - https://github.com/evrimai/python-client/blob/HEAD/README.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/authentication/evrim-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Intelligence
- Signals
- Data Enrichment
- Profiles
- Entity Resolution
- Defense
- Financial Services
- Government
---
