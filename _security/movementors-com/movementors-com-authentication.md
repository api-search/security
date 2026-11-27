---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: movementors-com-auth-api-openapi.yml
  format: yaml
  label: MoveMentors Auth API
  slug: movementors-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-auth-api-openapi.yml
- filename: movementors-com-bookings-api-openapi.yml
  format: yaml
  label: MoveMentors Bookings API
  slug: movementors-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-bookings-api-openapi.yml
- filename: movementors-com-classes-api-openapi.yml
  format: yaml
  label: MoveMentors Classes API
  slug: movementors-com-classes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-classes-api-openapi.yml
- filename: movementors-com-notifications-api-openapi.yml
  format: yaml
  label: MoveMentors Notifications API
  slug: movementors-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-notifications-api-openapi.yml
- filename: movementors-com-public-api-openapi.yml
  format: yaml
  label: MoveMentors Public API
  slug: movementors-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-public-api-openapi.yml
- filename: movementors-com-public-api-v1-api-openapi.yml
  format: yaml
  label: MoveMentors Public API v1 API
  slug: movementors-com-public-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-public-api-v1-api-openapi.yml
- filename: movementors-com-push-api-openapi.yml
  format: yaml
  label: MoveMentors Push API
  slug: movementors-com-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-push-api-openapi.yml
- filename: movementors-com-reviews-api-openapi.yml
  format: yaml
  label: MoveMentors Reviews API
  slug: movementors-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-reviews-api-openapi.yml
- filename: movementors-com-search-api-openapi.yml
  format: yaml
  label: MoveMentors Search API
  slug: movementors-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-search-api-openapi.yml
- filename: movementors-com-settings-api-openapi.yml
  format: yaml
  label: MoveMentors Settings API
  slug: movementors-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-settings-api-openapi.yml
- filename: movementors-com-upload-api-openapi.yml
  format: yaml
  label: MoveMentors Upload API
  slug: movementors-com-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movementors-com/openapi/movementors-com-upload-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: MoveMentors Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoveMentors secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MoveMentors
provider_slug: movementors-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Short-lived access token (15 min) obtained from POST /api/auth/token. Refresh via POST /api/auth/token/refresh.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/movementors-com-openapi.json
  type: http
- description: NextAuth HttpOnly session cookie. Web-only; mobile clients should use BearerAuth instead.
  in: cookie
  name: CookieAuth
  parameter: authjs.session-token
  sources:
  - openapi/movementors-com-openapi.json
  type: apiKey
slug: movementors-com-authentication
source_filename: movementors-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/movementors-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Short-lived access token (15 min) obtained from POST /api/auth/token. Refresh\n    via POST /api/auth/token/refresh.\n  sources:\n  - openapi/movementors-com-openapi.json\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: authjs.session-token\n  description: NextAuth HttpOnly session cookie. Web-only; mobile clients should use BearerAuth\n    instead.\n  sources:\n  - openapi/movementors-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/movementors-com/authentication/movementors-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Wellness
- Booking
- Yoga
- Pilates
- Independent
---
