---
api_key_in: []
api_specs:
- filename: pinnacle-asyncapi.yml
  format: yaml
  label: Pinnacle Lines API
  slug: pinnacle-lines-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-asyncapi.yml
- filename: pinnacle-cancellationreasons-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Cancellationreasons API'
  slug: pinnacle-cancellationreasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-cancellationreasons-api-openapi.yml
- filename: pinnacle-currencies-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Currencies API'
  slug: pinnacle-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-currencies-api-openapi.yml
- filename: pinnacle-fixtures-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Fixtures API'
  slug: pinnacle-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-fixtures-api-openapi.yml
- filename: pinnacle-inrunning-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Inrunning API'
  slug: pinnacle-inrunning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-inrunning-api-openapi.yml
- filename: pinnacle-leagues-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Leagues API'
  slug: pinnacle-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-leagues-api-openapi.yml
- filename: pinnacle-line-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Line API'
  slug: pinnacle-line-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-line-api-openapi.yml
- filename: pinnacle-odds-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Odds API'
  slug: pinnacle-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-odds-api-openapi.yml
- filename: pinnacle-periods-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Periods API'
  slug: pinnacle-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-periods-api-openapi.yml
- filename: pinnacle-sports-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Sports API'
  slug: pinnacle-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-sports-api-openapi.yml
- filename: pinnacle-teaser-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Teaser API'
  slug: pinnacle-teaser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-teaser-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pinnacle Authentication
name_suffix: Authentication
oauth_flows: []
overview: ' Pinnacle Sports Betting secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.'
provider_name: ' Pinnacle Sports Betting'
provider_slug: pinnacle
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/pinnacle-openapi.yml
  type: http
slug: pinnacle-authentication
source_filename: pinnacle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pinnacle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/pinnacle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/authentication/pinnacle-authentication.yml
summary_line: http · 1 scheme
tags:
- Gambling
- Sports Betting
---
