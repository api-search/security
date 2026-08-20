---
api_key_in:
- header
api_specs:
- filename: genlogs-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Alerts API
  slug: genlogs-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-alerts-api-openapi.yml
- filename: genlogs-auth-api-openapi.yml
  format: yaml
  label: GenLogs auth API
  slug: genlogs-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-auth-api-openapi.yml
- filename: genlogs-carrier-api-openapi.yml
  format: yaml
  label: GenLogs Carrier API
  slug: genlogs-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-carrier-api-openapi.yml
- filename: genlogs-carrier-vetting-api-openapi.yml
  format: yaml
  label: GenLogs carrier-vetting API
  slug: genlogs-carrier-vetting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-carrier-vetting-api-openapi.yml
- filename: genlogs-compliance-rules-api-openapi.yml
  format: yaml
  label: GenLogs Compliance Rules API
  slug: genlogs-compliance-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-compliance-rules-api-openapi.yml
- filename: genlogs-facilities-api-openapi.yml
  format: yaml
  label: GenLogs Facilities API
  slug: genlogs-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-facilities-api-openapi.yml
- filename: genlogs-mismatch-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Mismatch alerts API
  slug: genlogs-mismatch-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-mismatch-alerts-api-openapi.yml
- filename: genlogs-onboarded-carriers-api-openapi.yml
  format: yaml
  label: GenLogs Onboarded Carriers API
  slug: genlogs-onboarded-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-onboarded-carriers-api-openapi.yml
- filename: genlogs-shipper-api-openapi.yml
  format: yaml
  label: GenLogs Shipper API
  slug: genlogs-shipper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-shipper-api-openapi.yml
- filename: genlogs-webhook-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Webhook Alerts API
  slug: genlogs-webhook-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-webhook-alerts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Genlogs Authentication
name_suffix: Authentication
oauth_flows: []
overview: GenLogs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GenLogs
provider_slug: genlogs
scheme_count: 2
schemes:
- description: API key provided by GenLogs. Required on every request.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/genlogs-openapi.yml
  type: apiKey
- description: Short-lived access token obtained from POST /auth/token (or refreshed via /auth/token/refresh).
  in: header
  name: AccessToken
  parameter: Access-Token
  sources:
  - openapi/genlogs-openapi.yml
  type: apiKey
slug: genlogs-authentication
source_filename: genlogs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/genlogs-openapi.yml\ndocs: https://docs.genlogs.io/getting-started\nmodel: >-\n  Two-factor request auth: every request carries the static x-api-key header AND a\n  short-lived Access-Token header. The Access-Token is minted by POST /auth/token using\n  email + password credentials issued by the GenLogs customer-success team, and expires\n  (TokenSchema.expires). A refresh token is returned by /auth/token/refresh but the docs\n  note it is not usable at this time - create a new token after expiry. Per-endpoint access\n  is further gated by named permissions granted to the key/customer (403 on missing permission).\ntoken_flow:\n  create: POST https://api.genlogs.io/auth/token\n  refresh: POST https://api.genlogs.io/auth/token/refresh\n  headers_required: [x-api-key, Access-Token]\npermissions:\n  note: Named per-endpoint permissions; a missing permission returns 403 Forbidden.\n  examples:\n  - verifier-carrier\n  -\
  \ realtime-api\n  - external-api-carrier-recommendation\n  - external-api-carrier-profile\n  - external-api-carrier-contacts\n  - external-api-carrier-iss-score\n  - external-api-shipper-lanes\n  - external-api-shipper-facilities\n  - external-api-shipper-network-map\n  - external-api-compliance-rules\n  - external-api-update-compliance-rules\n  - external-api-get-onboarded-carrier-contact\n  - external-api-create-onboarded-carrier-contact\n  - external-api-update-onboarded-carrier-contact\n  - external-api-delete-onboarded-carrier-contact\n  - external-api-mismatch-observations\n  - external-api-get-all-company-alerts\n  - external-api-get-webhook-list\n  - external-api-delete-alert-webhook-endpoint\n  - create-alert-endpoint\n  - edit-alert-endpoint\n  - create-alert-webhook-endpoint\n  - edit-alert-webhook-endpoint\n  - test-alert-webhook-endpoint\n  - run-summary-alert\n  - admin\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n\
  \  in: header\n  parameter: x-api-key\n  description: API key provided by GenLogs. Required on every request.\n  sources:\n  - openapi/genlogs-openapi.yml\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: Access-Token\n  description: Short-lived access token obtained from POST /auth/token (or refreshed via /auth/token/refresh).\n  sources:\n  - openapi/genlogs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/authentication/genlogs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Logistics
- Freight
- Trucking
- Supply Chain
- Carrier Intelligence
- Fleet
- Transportation
- Insurance
- Fraud Detection
- Webhook
- Geospatial
---
