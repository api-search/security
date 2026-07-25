---
api_key_in:
- header
api_specs:
- filename: cable-alerts-api-openapi.yml
  format: yaml
  label: Cable alerts API
  slug: cable-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-alerts-api-openapi.yml
- filename: cable-authentication-api-openapi.yml
  format: yaml
  label: Cable authentication API
  slug: cable-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-authentication-api-openapi.yml
- filename: cable-business-api-openapi.yml
  format: yaml
  label: Cable business API
  slug: cable-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-business-api-openapi.yml
- filename: cable-checks-api-openapi.yml
  format: yaml
  label: Cable checks API
  slug: cable-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-checks-api-openapi.yml
- filename: cable-company-api-openapi.yml
  format: yaml
  label: Cable company API
  slug: cable-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-company-api-openapi.yml
- filename: cable-customersar-api-openapi.yml
  format: yaml
  label: Cable customerSar API
  slug: cable-customersar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-customersar-api-openapi.yml
- filename: cable-helper-api-openapi.yml
  format: yaml
  label: Cable helper API
  slug: cable-helper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-helper-api-openapi.yml
- filename: cable-identityverification-api-openapi.yml
  format: yaml
  label: Cable identityVerification API
  slug: cable-identityverification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-identityverification-api-openapi.yml
- filename: cable-onboardingflow-api-openapi.yml
  format: yaml
  label: Cable onboardingFlow API
  slug: cable-onboardingflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-onboardingflow-api-openapi.yml
- filename: cable-person-api-openapi.yml
  format: yaml
  label: Cable person API
  slug: cable-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-person-api-openapi.yml
- filename: cable-retail-api-openapi.yml
  format: yaml
  label: Cable retail API
  slug: cable-retail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-retail-api-openapi.yml
- filename: cable-riskassessment-api-openapi.yml
  format: yaml
  label: Cable riskAssessment API
  slug: cable-riskassessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-riskassessment-api-openapi.yml
- filename: cable-screening-api-openapi.yml
  format: yaml
  label: Cable screening API
  slug: cable-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-screening-api-openapi.yml
- filename: cable-suspiciousactivities-api-openapi.yml
  format: yaml
  label: Cable suspiciousActivities API
  slug: cable-suspiciousactivities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-suspiciousactivities-api-openapi.yml
- filename: cable-transactionalerts-api-openapi.yml
  format: yaml
  label: Cable transactionAlerts API
  slug: cable-transactionalerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transactionalerts-api-openapi.yml
- filename: cable-transactionchecks-api-openapi.yml
  format: yaml
  label: Cable transactionChecks API
  slug: cable-transactionchecks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transactionchecks-api-openapi.yml
- filename: cable-transactions-api-openapi.yml
  format: yaml
  label: Cable transactions API
  slug: cable-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transactions-api-openapi.yml
- filename: cable-transactionsuspiciousactivities-api-openapi.yml
  format: yaml
  label: Cable transactionSuspiciousActivities API
  slug: cable-transactionsuspiciousactivities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transactionsuspiciousactivities-api-openapi.yml
- filename: cable-upload-api-openapi.yml
  format: yaml
  label: Cable upload API
  slug: cable-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-upload-api-openapi.yml
- filename: cable-utilities-api-openapi.yml
  format: yaml
  label: Cable utilities API
  slug: cable-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-utilities-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cable secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cable
provider_slug: cable
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  note: refresh/auth token used to request an access token; also carries the bearer access token
  parameter: Authorization
  sources:
  - openapi/cable-api-reference-openapi-original.yml
  - openapi/cable-transaction-data-api-openapi-original.yml
  type: apiKey
- name: BearerAuth
  note: short-lived scoped access token returned by POST /auth/token
  scheme: bearer
  sources:
  - openapi/cable-api-reference-openapi-original.yml
  - openapi/cable-transaction-data-api-openapi-original.yml
  type: http
- in: header
  name: isValidAPIKey
  note: API key auth on the Customer Data API (v1)
  parameter: x-api-key
  sources:
  - openapi/cable-customer-data-api-openapi-original.yml
  type: apiKey
slug: cable-authentication
source_filename: cable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cable-api-reference-openapi-original.yml, openapi/cable-customer-data-api-openapi-original.yml,\n  openapi/cable-transaction-data-api-openapi-original.yml\ndocs: https://docs.cable.tech/api-documentation/api-reference/authentication/request-token\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: >-\n    Two-legged token exchange. Cable issues each customer a long-lived refresh/auth token\n    (an API key). The client presents that key in the Authorization header to POST /auth/token,\n    receiving a short-lived scoped bearer access token (expiry 300-86400s, requested via\n    expiry_seconds). That access token is then sent as a Bearer token on subsequent API calls.\n    A new access token cannot be requested using an existing access token.\nscopes_model:\n  described: true\n  shape: \"AccessTokenScope { organization_id, scopes[] }\"\n  example_scopes:\n  - transactions:write\n  note: >-\n\
  \    Tokens are scoped to an organization_id plus a list of string scopes (e.g. transactions:write).\n    Scopes are conveyed in the token request/response body, not via an OAuth2 securityScheme, so no\n    separate scopes/ artifact is emitted; the scope surface is documented here.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  note: refresh/auth token used to request an access token; also carries the bearer access token\n  sources:\n  - openapi/cable-api-reference-openapi-original.yml\n  - openapi/cable-transaction-data-api-openapi-original.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  note: short-lived scoped access token returned by POST /auth/token\n  sources:\n  - openapi/cable-api-reference-openapi-original.yml\n  - openapi/cable-transaction-data-api-openapi-original.yml\n- name: isValidAPIKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  note: API key auth on the Customer Data API (v1)\n  sources:\n  - openapi/cable-customer-data-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/authentication/cable-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Compliance
- Financial Crime
- RegTech
- Anti-Money Laundering
- Transaction Monitoring
- Screening
- Risk Assessment
- Banking
- Fintech
---
