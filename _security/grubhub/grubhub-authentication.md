---
api_key_in:
- header
api_specs:
- filename: grubhub-delivery-status-api-openapi.yml
  format: yaml
  label: grubhub Delivery Status API
  slug: grubhub-delivery-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-status-api-openapi.yml
- filename: grubhub-driver-communication-api-openapi.yml
  format: yaml
  label: grubhub Driver Communication API
  slug: grubhub-driver-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-driver-communication-api-openapi.yml
- filename: grubhub-issue-reporting-api-openapi.yml
  format: yaml
  label: grubhub Issue Reporting API
  slug: grubhub-issue-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-issue-reporting-api-openapi.yml
- filename: grubhub-menu-ingestion-api-openapi.yml
  format: yaml
  label: grubhub Menu Ingestion API
  slug: grubhub-menu-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-ingestion-api-openapi.yml
- filename: grubhub-menu-retrieval-api-openapi.yml
  format: yaml
  label: grubhub Menu Retrieval API
  slug: grubhub-menu-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-retrieval-api-openapi.yml
- filename: grubhub-menu-schedule-overrides-api-openapi.yml
  format: yaml
  label: grubhub Menu Schedule Overrides API
  slug: grubhub-menu-schedule-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-schedule-overrides-api-openapi.yml
- filename: grubhub-merchant-eligibility-api-openapi.yml
  format: yaml
  label: grubhub Merchant Eligibility API
  slug: grubhub-merchant-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-eligibility-api-openapi.yml
- filename: grubhub-merchant-onboarding-api-openapi.yml
  format: yaml
  label: grubhub Merchant Onboarding API
  slug: grubhub-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-onboarding-api-openapi.yml
- filename: grubhub-merchant-properties-api-openapi.yml
  format: yaml
  label: grubhub Merchant Properties API
  slug: grubhub-merchant-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-properties-api-openapi.yml
- filename: grubhub-merchant-status-api-openapi.yml
  format: yaml
  label: grubhub Merchant Status API
  slug: grubhub-merchant-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-status-api-openapi.yml
- filename: grubhub-merchants-api-openapi.yml
  format: yaml
  label: grubhub Merchants API
  slug: grubhub-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchants-api-openapi.yml
- filename: grubhub-order-change-requests-api-openapi.yml
  format: yaml
  label: grubhub Order Change Requests API
  slug: grubhub-order-change-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-order-change-requests-api-openapi.yml
- filename: grubhub-order-polling-api-openapi.yml
  format: yaml
  label: grubhub Order Polling API
  slug: grubhub-order-polling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-order-polling-api-openapi.yml
- filename: grubhub-order-status-api-openapi.yml
  format: yaml
  label: grubhub Order Status API
  slug: grubhub-order-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-order-status-api-openapi.yml
- filename: grubhub-orders-api-openapi.yml
  format: yaml
  label: grubhub Orders API
  slug: grubhub-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-api-openapi.yml
- filename: grubhub-schedule-overrides-api-openapi.yml
  format: yaml
  label: grubhub Schedule Overrides API
  slug: grubhub-schedule-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-schedule-overrides-api-openapi.yml
- filename: grubhub-schedules-api-openapi.yml
  format: yaml
  label: grubhub Schedules API
  slug: grubhub-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-schedules-api-openapi.yml
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
