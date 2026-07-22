---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nymcard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nymcard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nymcard
provider_slug: nymcard
scheme_count: 1
schemes:
- description: The nCore API uses standard API-key authentication. After signing up on the nCore platform you receive a static API key whose value does not change. It must be supplied in the `apikey` request header on every call. All API traffic is served only over TLS (HTTPS).
  in: header
  name: apikey
  parameter_name: apikey
  sources:
  - docs.nymcard.com/get-started/api-core-principles
  type: apiKey
slug: nymcard-authentication
source_filename: nymcard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nymcard.com/get-started/api-core-principles.md\ndocs: https://docs.nymcard.com/get-started/api-core-principles\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter_name: apikey\n  description: >-\n    The nCore API uses standard API-key authentication. After signing up on the\n    nCore platform you receive a static API key whose value does not change. It\n    must be supplied in the `apikey` request header on every call. All API\n    traffic is served only over TLS (HTTPS).\n  sources: [docs.nymcard.com/get-started/api-core-principles]\nnotes: >-\n  Webhook callbacks from nCore to your endpoint use HTTP Basic Auth (base64\n  encoded) in the notification header — see asyncapi/nymcard-webhooks.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nymcard/refs/heads/main/authentication/nymcard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- Card Issuing
- Banking as a Service
- Fintech
- Embedded Finance
- MENA
---
