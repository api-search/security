---
api_key_in: []
api_specs:
- filename: giftbit-brands-api-openapi.yml
  format: yaml
  label: Giftbit Brands API
  slug: giftbit-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-brands-api-openapi.yml
- filename: giftbit-campaigns-api-openapi.yml
  format: yaml
  label: Giftbit Campaigns API
  slug: giftbit-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-campaigns-api-openapi.yml
- filename: giftbit-direct-links-api-openapi.yml
  format: yaml
  label: Giftbit Direct Links API
  slug: giftbit-direct-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-direct-links-api-openapi.yml
- filename: giftbit-embedded-rewards-api-openapi.yml
  format: yaml
  label: Giftbit Embedded Rewards API
  slug: giftbit-embedded-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-embedded-rewards-api-openapi.yml
- filename: giftbit-funds-api-openapi.yml
  format: yaml
  label: Giftbit Funds API
  slug: giftbit-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-funds-api-openapi.yml
- filename: giftbit-ping-api-openapi.yml
  format: yaml
  label: Giftbit Ping API
  slug: giftbit-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-ping-api-openapi.yml
- filename: giftbit-regions-api-openapi.yml
  format: yaml
  label: Giftbit Regions API
  slug: giftbit-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-regions-api-openapi.yml
- filename: giftbit-rewards-api-openapi.yml
  format: yaml
  label: Giftbit Rewards API
  slug: giftbit-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-rewards-api-openapi.yml
- filename: giftbit-shortlinks-api-openapi.yml
  format: yaml
  label: Giftbit Shortlinks API
  slug: giftbit-shortlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-shortlinks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Giftbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Giftbit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Giftbit
provider_slug: giftbit
scheme_count: 1
schemes:
- description: Authenticate by sending your API token prefixed with "Bearer " in the Authorization HTTP header. Generate tokens from your Giftbit account under Account -> API keys.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/giftbit-openapi.yml
  type: http
slug: giftbit-authentication
source_filename: giftbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/giftbit-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate by sending your API token prefixed with \"Bearer \" in the Authorization\n    HTTP header. Generate tokens from your Giftbit account under Account -> API keys.\n  sources:\n  - openapi/giftbit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/authentication/giftbit-authentication.yml
summary_line: http · 1 scheme
tags:
- Gift Cards
- Digital Rewards
- Incentives
- Payments
- Reward Distribution
- Prepaid Cards
---
