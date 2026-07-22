---
api_key_in:
- header
api_specs:
- filename: postman.yaml
  format: yaml
  label: Qover Embedded Insurance API
  slug: qover-embedded-insurance-api
  spec_type: Postman
  url: https://docs.qover.com/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Qover Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qover secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qover
provider_slug: qover
scheme_count: 1
schemes:
- description: 'Qover''s REST API authenticates with an API key that must be included in the header of every request. Each API key is a unique identifier that acts as a secure access token authenticating and authorizing the request. Keys are issued per partner/project: Qover first grants a Sandbox API key, then - after review and testing - provides a Production key through a secure protocol. Keys must be kept confidential and never committed to public repositories or client-side code.'
  in: header
  name: ApiKey
  sources:
  - postman:docs.qover.com (Qover API collection)
  type: apiKey
slug: qover-authentication
source_filename: qover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.qover.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  description: >-\n    Qover's REST API authenticates with an API key that must be included in the\n    header of every request. Each API key is a unique identifier that acts as a\n    secure access token authenticating and authorizing the request. Keys are\n    issued per partner/project: Qover first grants a Sandbox API key, then - after\n    review and testing - provides a Production key through a secure protocol.\n    Keys must be kept confidential and never committed to public repositories or\n    client-side code.\n  sources:\n  - postman:docs.qover.com (Qover API collection)\nwebhook_authentication:\n  description: >-\n    Outbound webhooks (claim status changes) support configurable authentication\n    on the receiving endpoint.\n  mechanisms:\n  - basic (username/password)\n\
  \  - api-key (header or query parameter)\n  - bearer token\nnotes:\n- API keys are shared privately during onboarding; there is no self-serve key issuance.\n- Request an API key at https://www.qover.com/api-access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qover/refs/heads/main/authentication/qover-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Insurtech
- Insurance
- Embedded Insurance
- Claims
- Policy
- API
- Fintech
- Belgium
---
