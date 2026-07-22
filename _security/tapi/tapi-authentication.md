---
api_key_in: []
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Tapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tapi secures its APIs with token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tapi
provider_slug: tapi
scheme_count: 1
schemes:
- name: login
  obtained_via: https://developers.tapila.cloud/docs/api-reference/login/login
  sources:
  - docs
  type: token
slug: tapi-authentication
source_filename: tapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.tapila.cloud/docs/api-reference/login/login\ndocs: https://developers.tapila.cloud/docs/api-reference/login/login\nsummary:\n  types: [token]\n  model: login-issued-token\n  description: >-\n    Tapi exposes a dedicated Login service. Clients authenticate against the login\n    endpoint with their issued credentials and receive an access token, which is\n    then presented on subsequent calls to the Companies, Services, Recharges,\n    Subscriptions and Agenda endpoints.\nschemes:\n  - name: login\n    type: token\n    obtained_via: https://developers.tapila.cloud/docs/api-reference/login/login\n    sources: [docs]\nnotes: >-\n  Tapi does not publish an OpenAPI definition, so this profile is derived from the\n  developer documentation rather than mechanically from securitySchemes. The exact\n  token header name, token lifetime and refresh semantics are documented on the\n  client-rendered developer portal\
  \ and were not captured verbatim in this pass.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapi/refs/heads/main/authentication/tapi-authentication.yml
summary_line: token · 1 scheme
tags:
- Company
- Payments
- Bill Payments
- Fintech
- Latin America
- Recharges
- Gift Cards
- Financial Infrastructure
- Payment Network
---
