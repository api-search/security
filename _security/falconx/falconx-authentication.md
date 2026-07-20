---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Falconx Authentication
name_suffix: Authentication
oauth_flows: []
overview: FalconX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FalconX
provider_slug: falconx
scheme_count: 1
schemes:
- description: API-key credential issued to onboarded FalconX institutional clients, required on all api.falconx.io REST calls.
  name: ApiKey
  sources:
  - https://falconx.stoplight.io/docs/falconx-api/authentication
  type: apiKey
slug: falconx-authentication
source_filename: falconx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://falconx.stoplight.io/docs/falconx-api/authentication\ndocs: https://falconx.stoplight.io/docs/falconx-api/authentication\nnote: >-\n  FalconX exposes a private, institution-onboarded REST trading API at\n  https://api.falconx.io. The public developer portal documents an API-key\n  security scheme (scheme name \"ApiKey\"); unauthenticated requests to the API\n  host redirect to a login/authorization flow. Full request-signing details are\n  behind institutional onboarding and were not verified from a public spec, so\n  only the confirmed key-based model is recorded here.\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: ApiKey\n  type: apiKey\n  description: >-\n    API-key credential issued to onboarded FalconX institutional clients,\n    required on all api.falconx.io REST calls.\n  sources:\n  - https://falconx.stoplight.io/docs/falconx-api/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/falconx/refs/heads/main/authentication/falconx-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cryptocurrency
- Digital Assets
- Prime Brokerage
- Trading
- Institutional
- Financial Services
- Custody
- Derivatives
- OTC
---
