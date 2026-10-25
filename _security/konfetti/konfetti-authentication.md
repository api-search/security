---
anonymous_access: false
api_key_in: []
api_specs:
- filename: konfetti-account-api-openapi.yml
  format: yaml
  label: konfetti Account API
  slug: konfetti-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-account-api-openapi.yml
- filename: konfetti-auth-api-openapi.yml
  format: yaml
  label: konfetti Auth API
  slug: konfetti-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-auth-api-openapi.yml
- filename: konfetti-catalog-api-openapi.yml
  format: yaml
  label: konfetti Catalog API
  slug: konfetti-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-catalog-api-openapi.yml
- filename: konfetti-checkout-api-openapi.yml
  format: yaml
  label: konfetti Checkout API
  slug: konfetti-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-checkout-api-openapi.yml
- filename: konfetti-requests-api-openapi.yml
  format: yaml
  label: konfetti Requests API
  slug: konfetti-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/openapi/konfetti-requests-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Konfetti Authentication
name_suffix: Authentication
oauth_flows: []
overview: konfetti secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: konfetti
provider_slug: konfetti
scheme_count: 2
schemes:
- description: 'Access token obtained from POST /v1/oauth/token and sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/konfetti-account-api-openapi.yml
  - openapi/konfetti-auth-api-openapi.yml
  - openapi/konfetti-catalog-api-openapi.yml
  - openapi/konfetti-checkout-api-openapi.yml
  - openapi/konfetti-requests-api-openapi.yml
  type: http
- description: OAuth 2.0 token endpoint confirmed at /v1/oauth/token (League OAuth2 Server). No authorization endpoint, discovery document or scope reference is published, so no flows are enumerated here.
  flows: []
  name: oauth2
  sources:
  - openapi/konfetti-account-api-openapi.yml
  - openapi/konfetti-auth-api-openapi.yml
  - openapi/konfetti-catalog-api-openapi.yml
  - openapi/konfetti-checkout-api-openapi.yml
  - openapi/konfetti-requests-api-openapi.yml
  type: oauth2
slug: konfetti-authentication
source_filename: konfetti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/konfetti-account-api-openapi.yml, openapi/konfetti-auth-api-openapi.yml, openapi/konfetti-catalog-api-openapi.yml,\n  openapi/konfetti-checkout-api-openapi.yml, openapi/konfetti-requests-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token obtained from POST /v1/oauth/token and sent as `Authorization:\n    Bearer <token>`.'\n  sources:\n  - openapi/konfetti-account-api-openapi.yml\n  - openapi/konfetti-auth-api-openapi.yml\n  - openapi/konfetti-catalog-api-openapi.yml\n  - openapi/konfetti-checkout-api-openapi.yml\n  - openapi/konfetti-requests-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows: []\n  description: OAuth 2.0 token endpoint confirmed at /v1/oauth/token (League OAuth2 Server).\n    No authorization endpoint, discovery document or scope reference is published, so no flows\n    are enumerated here.\n  sources:\n\
  \  - openapi/konfetti-account-api-openapi.yml\n  - openapi/konfetti-auth-api-openapi.yml\n  - openapi/konfetti-catalog-api-openapi.yml\n  - openapi/konfetti-checkout-api-openapi.yml\n  - openapi/konfetti-requests-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konfetti/refs/heads/main/authentication/konfetti-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Marketplace
- Experience
- Booking
- Event
- Workshops
- Ticketing
- Gift Cards
- Travel And Leisure
- Germany
- Commerce
---
