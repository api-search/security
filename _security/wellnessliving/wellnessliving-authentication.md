---
api_key_in: []
api_specs:
- filename: wellnessliving-appointments-api-openapi.yml
  format: yaml
  label: WellnessLiving Appointments API
  slug: wellnessliving-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-appointments-api-openapi.yml
- filename: wellnessliving-authentication-api-openapi.yml
  format: yaml
  label: WellnessLiving Authentication API
  slug: wellnessliving-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-authentication-api-openapi.yml
- filename: wellnessliving-booking-api-openapi.yml
  format: yaml
  label: WellnessLiving Booking API
  slug: wellnessliving-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-booking-api-openapi.yml
- filename: wellnessliving-business-api-openapi.yml
  format: yaml
  label: WellnessLiving Business API
  slug: wellnessliving-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-business-api-openapi.yml
- filename: wellnessliving-catalog-api-openapi.yml
  format: yaml
  label: WellnessLiving Catalog API
  slug: wellnessliving-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-catalog-api-openapi.yml
- filename: wellnessliving-classes-api-openapi.yml
  format: yaml
  label: WellnessLiving Classes API
  slug: wellnessliving-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-classes-api-openapi.yml
- filename: wellnessliving-clients-api-openapi.yml
  format: yaml
  label: WellnessLiving Clients API
  slug: wellnessliving-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-clients-api-openapi.yml
- filename: wellnessliving-locations-api-openapi.yml
  format: yaml
  label: WellnessLiving Locations API
  slug: wellnessliving-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-locations-api-openapi.yml
- filename: wellnessliving-payments-api-openapi.yml
  format: yaml
  label: WellnessLiving Payments API
  slug: wellnessliving-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-payments-api-openapi.yml
- filename: wellnessliving-promotions-api-openapi.yml
  format: yaml
  label: WellnessLiving Promotions API
  slug: wellnessliving-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-promotions-api-openapi.yml
- filename: wellnessliving-reports-api-openapi.yml
  format: yaml
  label: WellnessLiving Reports API
  slug: wellnessliving-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-reports-api-openapi.yml
- filename: wellnessliving-reviews-api-openapi.yml
  format: yaml
  label: WellnessLiving Reviews API
  slug: wellnessliving-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-reviews-api-openapi.yml
- filename: wellnessliving-rewards-api-openapi.yml
  format: yaml
  label: WellnessLiving Rewards API
  slug: wellnessliving-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-rewards-api-openapi.yml
- filename: wellnessliving-staff-api-openapi.yml
  format: yaml
  label: WellnessLiving Staff API
  slug: wellnessliving-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-staff-api-openapi.yml
- filename: wellnessliving-websocket-api-openapi.yml
  format: yaml
  label: WellnessLiving WebSocket API
  slug: wellnessliving-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-websocket-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wellnessliving Authentication
name_suffix: Authentication
oauth_flows: []
overview: WellnessLiving secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WellnessLiving
provider_slug: wellnessliving
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'The officially published OpenAPI declares a JWT Bearer scheme: sign in via `POST /Core/Passport/Login/Enter/Enter.json`, then mint a token with `GET /Core/Passport/Enter/Jwt/JwtToken.json` and send it as `Authorization: Bearer <token>`. The underlying PHP/JS SDKs additionally support the legacy scheme: a registered Application ID + secret code sign a per-request HMAC (SHA3-based) placed in the `Au'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/wellnessliving-openapi.yml
  type: http
slug: wellnessliving-authentication
source_filename: wellnessliving-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wellnessliving-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'The officially published OpenAPI declares a JWT Bearer scheme: sign in via `POST\n    /Core/Passport/Login/Enter/Enter.json`, then mint a token with `GET /Core/Passport/Enter/Jwt/JwtToken.json`\n    and send it as `Authorization: Bearer <token>`. The underlying PHP/JS SDKs additionally\n    support the legacy scheme: a registered Application ID + secret code sign a per-request\n    HMAC (SHA3-based) placed in the `Au'\n  sources:\n  - openapi/wellnessliving-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/authentication/wellnessliving-authentication.yml
summary_line: http · 1 scheme
tags:
- Fitness
- Wellness
- Spa
- Business Management
- Scheduling
- Memberships
- Point of Sale
---
