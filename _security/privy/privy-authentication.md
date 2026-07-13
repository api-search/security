---
api_key_in: []
api_specs:
- filename: privy-openapi.yml
  format: yaml
  label: Privy REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/privy/refs/heads/main/openapi/privy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Privy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Privy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Privy
provider_slug: privy
scheme_count: 1
schemes:
- description: 'HTTP Basic auth using your Privy app ID as the username and your app

    secret as the password. Must be sent alongside the privy-app-id header.'
  name: appSecretAuth
  scheme: basic
  sources:
  - openapi/privy-openapi.yml
  type: http
slug: privy-authentication
source_filename: privy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/privy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: appSecretAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth using your Privy app ID as the username and your app\n    secret as the password. Must be sent alongside the privy-app-id header.\n  sources:\n  - openapi/privy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/privy/refs/heads/main/authentication/privy-authentication.yml
summary_line: http · 1 scheme
tags:
- Web3
- Wallets
- Authentication
- Embedded Wallets
- MPC
---
