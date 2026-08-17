---
api_key_in:
- query
- header
api_specs:
- filename: postman.yaml
  format: yaml
  label: LeadSquared REST API
  slug: rest-api
  spec_type: Postman
  url: https://apidocs.leadsquared.com/leadsquared-run-in-postman/
- filename: leadsquared-activities-api-openapi.yml
  format: yaml
  label: LeadSquared Activities API
  slug: leadsquared-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/openapi/leadsquared-activities-api-openapi.yml
- filename: leadsquared-leads-api-openapi.yml
  format: yaml
  label: LeadSquared Leads API
  slug: leadsquared-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/openapi/leadsquared-leads-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Leadsquared Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeadSquared secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeadSquared
provider_slug: leadsquared
scheme_count: 5
schemes:
- in: query
  name: AccessKeyAuth
  parameter: accessKey
  sources:
  - openapi/leadsquared-leads-api-openapi.yml
  - openapi/leadsquared-activities-api-openapi.yml
  type: apiKey
- in: query
  name: SecretKeyAuth
  parameter: secretKey
  sources:
  - openapi/leadsquared-leads-api-openapi.yml
  - openapi/leadsquared-activities-api-openapi.yml
  type: apiKey
- in: header
  name: AccessKeyHeaderAuth
  parameter: x-LSQ-AccessKey
  recommended: true
  sources:
  - https://apidocs.leadsquared.com/authentication/
  type: apiKey
- in: header
  name: SecretKeyHeaderAuth
  parameter: x-LSQ-SecretKey
  recommended: true
  sources:
  - https://apidocs.leadsquared.com/authentication/
  type: apiKey
- in: header
  name: AsyncApiKey
  note: Async submissions require x-api-key in addition to the accessKey/secretKey pair; the async Status API requires only x-api-key.
  parameter: x-api-key
  scope: Async API only (asyncapi.leadsquared.com)
  sources:
  - https://apidocs.leadsquared.com/async-api/
  type: apiKey
slug: leadsquared-authentication
source_filename: leadsquared-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://apidocs.leadsquared.com/authentication/\ndocs: https://apidocs.leadsquared.com/authentication/\nderived_baseline: openapi/leadsquared-leads-api-openapi.yml, openapi/leadsquared-activities-api-openapi.yml\nnote: >-\n  SEARCHED upgrade over the derived baseline. The OpenAPI in this repo declares only\n  the query-string form of the key pair; the documentation additionally publishes the\n  header form (x-LSQ-AccessKey / x-LSQ-SecretKey) and recommends it, and names the\n  operational constraints on the keys. No OAuth 2.0, no OpenID Connect, no bearer\n  tokens, no scopes, no refresh — so no scopes/ artifact is emitted for this provider.\nsummary:\n  types: [apiKey]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\n  https_required: true\nschemes:\n  - name: AccessKeyAuth\n    type: apiKey\n    in: query\n    parameter: accessKey\n    sources: [openapi/leadsquared-leads-api-openapi.yml,\
  \ openapi/leadsquared-activities-api-openapi.yml]\n  - name: SecretKeyAuth\n    type: apiKey\n    in: query\n    parameter: secretKey\n    sources: [openapi/leadsquared-leads-api-openapi.yml, openapi/leadsquared-activities-api-openapi.yml]\n  - name: AccessKeyHeaderAuth\n    type: apiKey\n    in: header\n    parameter: x-LSQ-AccessKey\n    recommended: true\n    sources: [https://apidocs.leadsquared.com/authentication/]\n  - name: SecretKeyHeaderAuth\n    type: apiKey\n    in: header\n    parameter: x-LSQ-SecretKey\n    recommended: true\n    sources: [https://apidocs.leadsquared.com/authentication/]\n  - name: AsyncApiKey\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    scope: Async API only (asyncapi.leadsquared.com)\n    sources: [https://apidocs.leadsquared.com/async-api/]\n    note: >-\n      Async submissions require x-api-key in addition to the accessKey/secretKey pair;\n      the async Status API requires only x-api-key.\nkey_management:\n  issued_at: My Account\
  \ > Settings > API and Webhooks\n  binding: individual admin user\n  rotation_policy: not published\n  expiry: none documented\n  constraints:\n    - Keys should belong to an active Admin user account.\n    - >-\n      Deactivating the user deactivates their API keys, which fails every integration\n      bound to them. This is the most common non-obvious 401 cause after the wrong\n      regional host.\ntransport:\n  https_only: true\n  quote: >-\n    \"All API requests must be made over HTTPS. Calls made using plain HTTP will fail.\"\n  query_string_warning: >-\n    LeadSquared accepts credentials in the query string. That places long-lived secrets\n    into URLs, proxy logs and browser history; the header form should be used instead.\nhost_binding:\n  regional: true\n  note: >-\n    Authentication is host-bound — a valid key pair sent to the wrong regional host\n    returns 401 with the correct host named in the error message. See\n    conventions/leadsquared-conventions.yml.\n  docs:\
  \ https://apidocs.leadsquared.com/api-host/\nportal_authentication:\n  note: >-\n    A separate authentication surface exists for LeadSquared Portals (self-service end\n    users): register, sign-in, OTP sign-in, password reset, auto-login tenant and\n    lead-level auth keys. It is end-user authentication, not API-client authentication.\n  docs: https://apidocs.leadsquared.com/portal-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/authentication/leadsquared-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Marketing Automation
- CRM
- Sales Automation
- Lead Management
- Customer Engagement
- Field Force Automation
---
