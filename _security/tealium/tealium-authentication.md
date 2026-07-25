---
api_key_in: []
api_specs:
- filename: tealium-auth-api-openapi.yml
  format: yaml
  label: Tealium Auth API
  slug: tealium-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-auth-api-openapi.yml
- filename: tealium-collect-api-openapi.yml
  format: yaml
  label: Tealium Collect API
  slug: tealium-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-collect-api-openapi.yml
- filename: tealium-customer-api-openapi.yml
  format: yaml
  label: Tealium Customer API
  slug: tealium-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-customer-api-openapi.yml
- filename: tealium-personalization-api-openapi.yml
  format: yaml
  label: Tealium Personalization API
  slug: tealium-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-personalization-api-openapi.yml
- filename: tealium-privacy-api-openapi.yml
  format: yaml
  label: Tealium Privacy API
  slug: tealium-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-privacy-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tealium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tealium secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tealium
provider_slug: tealium
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT bearer token obtained from the Authentication API (/v3/auth/accounts/{account}/profiles/{profile}). Tokens are valid for 30 minutes. Do not generate a new token for every call — reuse until expiration.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tealium-collect-http-openapi.yml
  - openapi/tealium-visitor-privacy-openapi.yml
  - openapi/tealium-visitor-profile-openapi.yml
  type: http
slug: tealium-authentication
source_filename: tealium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tealium-collect-http-openapi.yml, openapi/tealium-visitor-privacy-openapi.yml,\n  openapi/tealium-visitor-profile-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token obtained from the Authentication API (/v3/auth/accounts/{account}/profiles/{profile}).\n    Tokens are valid for 30 minutes. Do not generate a new token for every call — reuse until\n    expiration.\n  sources:\n  - openapi/tealium-collect-http-openapi.yml\n  - openapi/tealium-visitor-privacy-openapi.yml\n  - openapi/tealium-visitor-profile-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/authentication/tealium-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Data Platform
- CDP
- Tag Management
- AudienceStream
- Real-Time Events
- Visitor Profiles
- Audience Segmentation
- Data Collection
- Privacy Compliance
- Personalization
---
