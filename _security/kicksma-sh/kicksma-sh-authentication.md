---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kicksma-sh-clubs-api-openapi.yml
  format: yaml
  label: Kicksmash Clubs API
  slug: kicksma-sh-clubs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-clubs-api-openapi.yml
- filename: kicksma-sh-coaches-api-openapi.yml
  format: yaml
  label: Kicksmash Coaches API
  slug: kicksma-sh-coaches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-coaches-api-openapi.yml
- filename: kicksma-sh-groups-api-openapi.yml
  format: yaml
  label: Kicksmash Groups API
  slug: kicksma-sh-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-groups-api-openapi.yml
- filename: kicksma-sh-keys-api-openapi.yml
  format: yaml
  label: Kicksmash Keys API
  slug: kicksma-sh-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-keys-api-openapi.yml
- filename: kicksma-sh-matches-api-openapi.yml
  format: yaml
  label: Kicksmash Matches API
  slug: kicksma-sh-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-matches-api-openapi.yml
- filename: kicksma-sh-schedules-api-openapi.yml
  format: yaml
  label: Kicksmash Schedules API
  slug: kicksma-sh-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-schedules-api-openapi.yml
- filename: kicksma-sh-series-api-openapi.yml
  format: yaml
  label: Kicksmash Series API
  slug: kicksma-sh-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-series-api-openapi.yml
- filename: kicksma-sh-venues-api-openapi.yml
  format: yaml
  label: Kicksmash Venues API
  slug: kicksma-sh-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-venues-api-openapi.yml
- filename: kicksma-sh-webhooks-api-openapi.yml
  format: yaml
  label: Kicksmash Webhooks API
  slug: kicksma-sh-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kicksma-sh/openapi/kicksma-sh-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kicksmash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kicksmash secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kicksmash
provider_slug: kicksma-sh
scheme_count: 1
schemes:
- description: Optional for writes, required for webhooks. Keys start with ks_live_.
  name: bearer
  scheme: bearer
  sources:
  - openapi/kicksma-sh-openapi.json
  type: http
slug: kicksma-sh-authentication
source_filename: kicksma-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/kicksma-sh-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Optional for writes, required for webhooks. Keys start with ks_live_.\n  sources:\n  - openapi/kicksma-sh-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kicksma-sh/authentication/kicksma-sh-authentication.yml
summary_line: http · 1 scheme
tags:
- Padel
- Sports
- Matchmaking
- Mobile App
- Social
---
