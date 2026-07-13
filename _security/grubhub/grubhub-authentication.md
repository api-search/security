---
api_key_in:
- header
api_specs:
- filename: grubhub-menu-openapi.yml
  format: yaml
  label: Grubhub Menu API
  slug: menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-openapi.yml
- filename: grubhub-orders-openapi.yml
  format: yaml
  label: Grubhub Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-openapi.yml
- filename: grubhub-merchant-data-openapi.yml
  format: yaml
  label: Grubhub Merchant Data API
  slug: merchant-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-data-openapi.yml
- filename: grubhub-merchant-schedules-openapi.yml
  format: yaml
  label: Grubhub Merchant Schedules API
  slug: merchant-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-schedules-openapi.yml
- filename: grubhub-deliveries-openapi.yml
  format: yaml
  label: Grubhub Deliveries API
  slug: deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-deliveries-openapi.yml
- filename: grubhub-onboarding-openapi.yml
  format: yaml
  label: Grubhub Onboarding API
  slug: onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-onboarding-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Grubhub Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: grubhub secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: grubhub
provider_slug: grubhub
scheme_count: 2
schemes:
- description: HMAC-based authentication. Every request must include X-GH-PARTNER-KEY and an Authorization header with MAC authentication details.
  in: header
  name: hmacAuth
  parameter: Authorization
  sources:
  - openapi/grubhub-deliveries-openapi.yml
  - openapi/grubhub-menu-openapi.yml
  - openapi/grubhub-merchant-data-openapi.yml
  - openapi/grubhub-merchant-schedules-openapi.yml
  - openapi/grubhub-orders-openapi.yml
  type: apiKey
- description: OAuth 2.0 authentication for the Onboarding API. Partners use OAuth to authenticate merchant onboarding operations.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth2/direct/auth
  name: oauthAuth
  sources:
  - openapi/grubhub-onboarding-openapi.yml
  type: oauth2
slug: grubhub-authentication
source_filename: grubhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/grubhub-deliveries-openapi.yml, openapi/grubhub-menu-openapi.yml, openapi/grubhub-merchant-data-openapi.yml,\n  openapi/grubhub-merchant-schedules-openapi.yml, openapi/grubhub-onboarding-openapi.yml, openapi/grubhub-orders-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: hmacAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC-based authentication. Every request must include X-GH-PARTNER-KEY and an\n    Authorization header with MAC authentication details.\n  sources:\n  - openapi/grubhub-deliveries-openapi.yml\n  - openapi/grubhub-menu-openapi.yml\n  - openapi/grubhub-merchant-data-openapi.yml\n  - openapi/grubhub-merchant-schedules-openapi.yml\n  - openapi/grubhub-orders-openapi.yml\n- name: oauthAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/direct/auth\n \
  \   scopes: 0\n  description: OAuth 2.0 authentication for the Onboarding API. Partners use OAuth to authenticate\n    merchant onboarding operations.\n  sources:\n  - openapi/grubhub-onboarding-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/authentication/grubhub-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags: []
---
