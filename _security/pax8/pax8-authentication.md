---
api_key_in: []
api_specs:
- filename: pax8-authentication-openapi.json
  format: json
  label: Pax8 Authentication API
  slug: pax8-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-authentication-openapi.json
- filename: pax8-partner-endpoints-openapi.json
  format: json
  label: Pax8 Partner Endpoints
  slug: pax8-partner-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-partner-endpoints-openapi.json
- filename: pax8-quoting-endpoints-openapi.json
  format: json
  label: Pax8 Quoting Endpoints
  slug: pax8-quoting-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-quoting-endpoints-openapi.json
- filename: pax8-vendor-provisioning-endpoints-openapi.json
  format: json
  label: Pax8 Vendor Provisioning Endpoints
  slug: pax8-vendor-provisioning-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-vendor-provisioning-endpoints-openapi.json
- filename: pax8-vendor-usage-endpoints-openapi.json
  format: json
  label: Pax8 Vendor Usage Endpoints
  slug: pax8-vendor-usage-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-vendor-usage-endpoints-openapi.json
- filename: pax8-webhooks-api-openapi.json
  format: json
  label: Pax8 Webhooks API
  slug: pax8-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/openapi/pax8-webhooks-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pax8 Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pax8 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pax8
provider_slug: pax8
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://token-manager.pax8.com/oauth/token
  name: OAuth2
  sources:
  - openapi/pax8-authentication-openapi.json
  - openapi/pax8-partner-endpoints-openapi.json
  - openapi/pax8-vendor-provisioning-endpoints-openapi.json
  - openapi/pax8-vendor-usage-endpoints-openapi.json
  - openapi/pax8-webhooks-api-openapi.json
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pax8-quoting-endpoints-openapi.json
  type: http
slug: pax8-authentication
source_filename: pax8-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/pax8-authentication-openapi.json, openapi/pax8-partner-endpoints-openapi.json,\n  openapi/pax8-quoting-endpoints-openapi.json, openapi/pax8-vendor-provisioning-endpoints-openapi.json,\n  openapi/pax8-vendor-usage-endpoints-openapi.json, openapi/pax8-webhooks-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://token-manager.pax8.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/pax8-authentication-openapi.json\n  - openapi/pax8-partner-endpoints-openapi.json\n  - openapi/pax8-vendor-provisioning-endpoints-openapi.json\n  - openapi/pax8-vendor-usage-endpoints-openapi.json\n  - openapi/pax8-webhooks-api-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/pax8-quoting-endpoints-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pax8/refs/heads/main/authentication/pax8-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Enterprise
- Cloud Marketplace
- MSP
- Distribution
- Provisioning
- Billing
- Quoting
- Subscriptions
- Webhooks
---
