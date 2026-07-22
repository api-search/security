---
api_key_in:
- body
api_specs:
- filename: mirrortab-api-openapi.yml
  format: yaml
  label: MirrorTab API
  slug: mirrortab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirrortab/refs/heads/main/openapi/mirrortab-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mirrortab Authentication
name_suffix: Authentication
oauth_flows: []
overview: MirrorTab secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MirrorTab
provider_slug: mirrortab
scheme_count: 1
schemes:
- description: API key passed as the api_key field in the JSON request body. Obtain a key at https://mirrortab.com/API. Represented in the OpenAPI as an apiKey scheme because OpenAPI 3.0 cannot express a body-carried key.
  in: body
  name: apiKey
  parameter: api_key
  sources:
  - openapi/mirrortab-api-openapi.yml
  type: apiKey
slug: mirrortab-authentication
source_filename: mirrortab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mirrortab-api-openapi.yml\ndocs: https://github.com/MirrorTab/api_v1\nnotes: >-\n  MirrorTab authenticates every API call with a single API key sent as the\n  api_key field in the JSON request body (not a header or query parameter).\n  Keys are issued from the account dashboard at https://mirrortab.com/API. Free\n  accounts do not have API access; Enterprise and paid tiers gate the number of\n  concurrent sessions and maximum session duration. No OAuth, OIDC, or mTLS\n  surface is published.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - body\nschemes:\n- name: apiKey\n  type: apiKey\n  in: body\n  parameter: api_key\n  description: >-\n    API key passed as the api_key field in the JSON request body. Obtain a key\n    at https://mirrortab.com/API. Represented in the OpenAPI as an apiKey scheme\n    because OpenAPI 3.0 cannot express a body-carried key.\n  sources:\n  - openapi/mirrortab-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirrortab/refs/heads/main/authentication/mirrortab-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Security
- Cybersecurity
- Bot Mitigation
- Fraud Prevention
- Browser Isolation
- Anti-Automation
---
