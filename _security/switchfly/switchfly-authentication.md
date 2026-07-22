---
api_key_in: []
api_specs:
- filename: switchfly-loyalty-openapi.json
  format: json
  label: Switchfly Loyalty API
  slug: switchfly-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switchfly/refs/heads/main/openapi/switchfly-loyalty-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Switchfly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Switchfly secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Switchfly
provider_slug: switchfly
scheme_count: 2
schemes:
- description: Bearer token retrieved from OAuth 2 SSO token requests (POST /token). Used for traveler-facing loyalty actions such as fetching a profile and redeeming points.
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/switchfly-loyalty-openapi.json
  type: http
- description: Bearer token retrieved from a Machine-to-Machine OAuth 2 client_credentials token request (POST /admin/token). Used for administrative/M2M operations such as refunds.
  header: Authorization
  in: header
  name: adminBearerAuth
  scheme: bearer
  sources:
  - openapi/switchfly-loyalty-openapi.json
  type: http
slug: switchfly-authentication
source_filename: switchfly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.switchfly.com/dev/api-documentation/loyalty\nsummary:\n  types:\n  - http\n  - oauth2\n  overview: >-\n    The Switchfly Loyalty API authenticates via OAuth 2 SSO. Two HTTP bearer\n    schemes are declared in the OpenAPI: bearerAuth (traveler/SSO tokens) and\n    adminBearerAuth (machine-to-machine client-credentials tokens). Supported\n    grant types are authorization_code (with PKCE) and client_credentials.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token retrieved from OAuth 2 SSO token requests (POST /token). Used\n    for traveler-facing loyalty actions such as fetching a profile and redeeming\n    points.\n  in: header\n  header: Authorization\n  sources:\n  - openapi/switchfly-loyalty-openapi.json\n- name: adminBearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token retrieved from a Machine-to-Machine OAuth 2 client_credentials\n \
  \   token request (POST /admin/token). Used for administrative/M2M operations\n    such as refunds.\n  in: header\n  header: Authorization\n  sources:\n  - openapi/switchfly-loyalty-openapi.json\noauth2:\n  grant_types:\n  - authorization_code\n  - client_credentials\n  pkce: true\n  token_endpoint: POST /token\n  admin_token_endpoint: POST /admin/token\n  notes: >-\n    Clients with an existing internal SSO token can consolidate authorization via\n    the client_credentials flow using client_id and client_secret. Per-partner\n    token endpoints are served from a templated {domain}.switchfly.com host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/switchfly/refs/heads/main/authentication/switchfly-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Travel
- Loyalty
- Travel Technology
- Rewards
- Booking
- Dynamic Packaging
- White Label
- Points Redemption
- Travel Commerce
---
