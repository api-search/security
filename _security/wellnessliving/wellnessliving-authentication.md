---
api_key_in: []
api_specs:
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Clients API
  slug: clients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Classes & Schedules API
  slug: classes-schedule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Appointments API
  slug: appointments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Booking Wizard API
  slug: booking-wizard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Memberships & Passes API
  slug: memberships-passes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Staff API
  slug: staff
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Locations API
  slug: locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Business API
  slug: business
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Sales & Catalog API
  slug: sales-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Rewards & Loyalty API
  slug: rewards-loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Reviews API
  slug: reviews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Reports API
  slug: reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Real-Time Notifications API
  slug: realtime-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
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
