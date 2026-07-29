---
api_key_in: []
api_specs:
- filename: marriott-tip-internet-portal-api-openapi.json
  format: json
  label: Marriott TIP Internet Portal API
  slug: marriott-tip-internet-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-tip-internet-portal-api-openapi.json
- filename: marriott-loyalty-account-merge-api-openapi.json
  format: json
  label: Marriott Loyalty Account Merge API
  slug: marriott-loyalty-account-merge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-loyalty-account-merge-api-openapi.json
- filename: marriott-data-collection-api-openapi.json
  format: json
  label: Marriott Data Collection API
  slug: marriott-data-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-collection-api-openapi.json
- filename: marriott-commerce-payment-processor-api-openapi.json
  format: json
  label: Marriott Commerce Payment Processor API
  slug: marriott-commerce-payment-processor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-commerce-payment-processor-api-openapi.json
- filename: marriott-finance-status-notifier-api-openapi.json
  format: json
  label: Marriott Finance Status Notifier API
  slug: marriott-finance-status-notifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-finance-status-notifier-api-openapi.json
- filename: marriott-hotel-operations-ara-api-openapi.json
  format: json
  label: Marriott Hotel Operations ARA Preview Submit API
  slug: marriott-hotel-operations-ara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-hotel-operations-ara-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Marriott Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Marriott International secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Marriott International
provider_slug: marriott
scheme_count: 4
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/marriott-commerce-payment-processor-api-openapi.json
  - openapi/marriott-tip-internet-portal-api-openapi.json
  type: http
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/marriott-commerce-payment-processor-api-openapi.json
  - openapi/marriott-tip-internet-portal-api-openapi.json
  type: http
- flows:
  - authorizationUrl: /v3/ent-auth/sso/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: /v3/ent-auth/sso/token
  name: OAuth2
  sources:
  - openapi/marriott-commerce-payment-processor-api-openapi.json
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: http://example.com/oauth/token
  name: application
  sources:
  - openapi/marriott-finance-status-notifier-api-openapi.json
  type: oauth2
slug: marriott-authentication
source_filename: marriott-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: openapi/marriott-commerce-payment-processor-api-openapi.json, openapi/marriott-finance-status-notifier-api-openapi.json,\n  openapi/marriott-tip-internet-portal-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/marriott-commerce-payment-processor-api-openapi.json\n  - openapi/marriott-tip-internet-portal-api-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/marriott-commerce-payment-processor-api-openapi.json\n  - openapi/marriott-tip-internet-portal-api-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v3/ent-auth/sso/authorize\n    tokenUrl: /v3/ent-auth/sso/token\n    scopes: 1\n  sources:\n  - openapi/marriott-commerce-payment-processor-api-openapi.json\n\
  - name: application\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: http://example.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/marriott-finance-status-notifier-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/authentication/marriott-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Distribution
- Loyalty
- Short Term Rental
- Corporate Travel
---
