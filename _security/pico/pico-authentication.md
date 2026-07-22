---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pico secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pico
provider_slug: pico
scheme_count: 1
schemes:
- description: Every request to the Pico API must include an X-Api-Key header carrying an API access token. Tokens are generated in the Pico dashboard under Settings > Website by clicking "Request access token". No OAuth or scope surface is documented; access is a single account-level API key.
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - https://help.trypico.com/en/articles/5632118-using-the-pico-api
  type: apiKey
slug: pico-authentication
source_filename: pico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://help.trypico.com/en/articles/5632118-using-the-pico-api\ndocs: https://docs.trypico.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: >-\n    Every request to the Pico API must include an X-Api-Key header carrying an\n    API access token. Tokens are generated in the Pico dashboard under\n    Settings > Website by clicking \"Request access token\". No OAuth or scope\n    surface is documented; access is a single account-level API key.\n  sources:\n  - https://help.trypico.com/en/articles/5632118-using-the-pico-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pico/refs/heads/main/authentication/pico-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Creator Economy
- CRM
- Memberships
- Payments
- Email Marketing
- Newsletters
- Monetization
---
