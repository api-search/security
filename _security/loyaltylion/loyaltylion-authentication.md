---
api_key_in: []
api_specs:
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Customers API
  slug: loyaltylion-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Activities API
  slug: loyaltylion-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Points API
  slug: loyaltylion-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Rewards API
  slug: loyaltylion-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Redemptions API
  slug: loyaltylion-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Loyaltylion Authentication
name_suffix: Authentication
oauth_flows: []
overview: LoyaltyLion secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LoyaltyLion
provider_slug: loyaltylion
scheme_count: 2
schemes:
- description: Program API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/loyaltylion-openapi.yml
  type: http
- description: Deprecated token (username) and secret (password) over HTTP Basic auth, supported until 2027-01-10.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/loyaltylion-openapi.yml
  type: http
slug: loyaltylion-authentication
source_filename: loyaltylion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loyaltylion-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Program API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/loyaltylion-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Deprecated token (username) and secret (password) over HTTP Basic auth, supported\n    until 2027-01-10.\n  sources:\n  - openapi/loyaltylion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/authentication/loyaltylion-authentication.yml
summary_line: http · 2 schemes
tags:
- Loyalty
- Rewards
- E-commerce
- Points
- Shopify
- Retention
---
