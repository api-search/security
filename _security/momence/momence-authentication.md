---
api_key_in: []
api_specs:
- filename: momence-openapi.yml
  format: yaml
  label: Momence Authentication API
  slug: momence-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Members API
  slug: momence-host-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Sessions & Bookings API
  slug: momence-host-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Memberships API
  slug: momence-host-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Checkout & Sales API
  slug: momence-host-checkout-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Member Account API
  slug: momence-member-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Member Booking API
  slug: momence-member-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Momence Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Momence secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Momence
provider_slug: momence
scheme_count: 2
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  sources:
  - openapi/momence-openapi.yml
  type: oauth2
- description: Use your `client_id` as username and `client_secret` as password
  name: OAuth2ApiClient
  scheme: basic
  sources:
  - openapi/momence-openapi.yml
  type: http
slug: momence-authentication
source_filename: momence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/momence-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /api/v2/auth/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\n    scopes: 0\n  sources:\n  - openapi/momence-openapi.yml\n- name: OAuth2ApiClient\n  type: http\n  scheme: basic\n  description: Use your `client_id` as username and `client_secret` as password\n  sources:\n  - openapi/momence-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/authentication/momence-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fitness
- Wellness
- Studio Management
- Booking
- Scheduling
- Memberships
- Payments
- Class Management
---
