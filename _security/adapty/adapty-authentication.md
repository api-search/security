---
api_key_in:
- header
api_specs:
- filename: adapty-access-levels-api-openapi.yml
  format: yaml
  label: Adapty Access Levels API
  slug: adapty-access-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-access-levels-api-openapi.yml
- filename: adapty-integrations-api-openapi.yml
  format: yaml
  label: Adapty Integrations API
  slug: adapty-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-integrations-api-openapi.yml
- filename: adapty-paywalls-api-openapi.yml
  format: yaml
  label: Adapty Paywalls API
  slug: adapty-paywalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-paywalls-api-openapi.yml
- filename: adapty-profiles-api-openapi.yml
  format: yaml
  label: Adapty Profiles API
  slug: adapty-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-profiles-api-openapi.yml
- filename: adapty-purchases-api-openapi.yml
  format: yaml
  label: Adapty Purchases API
  slug: adapty-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-purchases-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Adapty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adapty secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adapty
provider_slug: adapty
scheme_count: 1
schemes:
- description: 'Secret API key passed as `Authorization: Api-Key <secret_live_...>`. Find your secret key in the Adapty dashboard under App Settings > API keys.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/adapty-openapi.yml
  type: apiKey
slug: adapty-authentication
source_filename: adapty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adapty-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Secret API key passed as `Authorization: Api-Key <secret_live_...>`. Find your\n    secret key in the Adapty dashboard under App Settings > API keys.'\n  sources:\n  - openapi/adapty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/authentication/adapty-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Mobile
- Subscriptions
- In-App Purchases
- Paywalls
- Analytics
---
