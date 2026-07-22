---
api_key_in: []
api_specs:
- filename: spotnana-auth-openapi-original.json
  format: json
  label: Spotnana Authentication API
  slug: spotnana-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-auth-openapi-original.json
- filename: spotnana-users-openapi-original.json
  format: json
  label: Spotnana Users API
  slug: spotnana-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-users-openapi-original.json
- filename: spotnana-company-openapi-original.json
  format: json
  label: Spotnana Company API
  slug: spotnana-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-company-openapi-original.json
- filename: spotnana-policy-openapi-original.json
  format: json
  label: Spotnana Policy API
  slug: spotnana-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-policy-openapi-original.json
- filename: spotnana-trip-openapi-original.json
  format: json
  label: Spotnana Trip API
  slug: spotnana-trip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-trip-openapi-original.json
- filename: spotnana-air-openapi-original.json
  format: json
  label: Spotnana Air API
  slug: spotnana-air-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-air-openapi-original.json
- filename: spotnana-hotel-openapi-original.json
  format: json
  label: Spotnana Hotel API
  slug: spotnana-hotel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-hotel-openapi-original.json
- filename: spotnana-event-openapi-original.json
  format: json
  label: Spotnana Event API
  slug: spotnana-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-event-openapi-original.json
- filename: spotnana-template-openapi-original.json
  format: json
  label: Spotnana Event Template API
  slug: spotnana-event-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-template-openapi-original.json
- filename: spotnana-payments-openapi-original.json
  format: json
  label: Spotnana Payments API
  slug: spotnana-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-payments-openapi-original.json
- filename: spotnana-document-openapi-original.json
  format: json
  label: Spotnana Document API
  slug: spotnana-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-document-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Spotnana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spotnana secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spotnana
provider_slug: spotnana
scheme_count: 1
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/spotnana-air-openapi-original.json
  - openapi/spotnana-auth-openapi-original.json
  - openapi/spotnana-company-openapi-original.json
  - openapi/spotnana-document-openapi-original.json
  - openapi/spotnana-event-openapi-original.json
  - openapi/spotnana-hotel-openapi-original.json
  - openapi/spotnana-payments-openapi-original.json
  - openapi/spotnana-policy-openapi-original.json
  - openapi/spotnana-template-openapi-original.json
  - openapi/spotnana-trip-openapi-original.json
  - openapi/spotnana-users-openapi-original.json
  type: http
slug: spotnana-authentication
source_filename: spotnana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spotnana-*-openapi-original.json (11 specs)\ndocs: https://developer.spotnana.com/openapi/authapi\noauth2:\n  token_endpoint: POST /v2/auth/oauth2-token\n  grant_types:\n    - client_credentials\n    - urn:ietf:params:oauth:grant-type:token-exchange\n  request_media_type: application/x-www-form-urlencoded\n  request_fields: [grant_type, client_id, client_secret, audience, subject_token, subject_token_type]\n  audience_example: https://apis.spotnana.com/v2\n  response_fields: [access_token, expires_in, token_type, refresh_token, scope]\n  api_user_management:\n    - createApiUser (POST /v2/api-users)\n    - getApiUsers (GET /v2/api-users)\n    - rotateClientSecret (POST /v2/api-users/rotate)\n    - deleteApiUser (POST /v2/api-users/revoke)\n  notes: >-\n    Every API is protected by an HTTP Bearer token. The token is minted by exchanging\n    an API user's client_id/client_secret at the OAuth2 token endpoint (client_credentials),\n\
  \    or by RFC 8693 token-exchange to act on behalf of a subject. Tokens are short-lived\n    (expires_in) and refreshable; client secrets can be rotated and revoked.\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/spotnana-air-openapi-original.json\n  - openapi/spotnana-auth-openapi-original.json\n  - openapi/spotnana-company-openapi-original.json\n  - openapi/spotnana-document-openapi-original.json\n  - openapi/spotnana-event-openapi-original.json\n  - openapi/spotnana-hotel-openapi-original.json\n  - openapi/spotnana-payments-openapi-original.json\n  - openapi/spotnana-policy-openapi-original.json\n  - openapi/spotnana-template-openapi-original.json\n  - openapi/spotnana-trip-openapi-original.json\n  - openapi/spotnana-users-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/authentication/spotnana-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- Travel
- Corporate Travel
- Travel Management
- Booking
- Air
- Hotel
- Payments
- Travel as a Service
---
