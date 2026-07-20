---
api_key_in:
- header
api_specs:
- filename: leadspace-enrichment-openapi.yml
  format: yaml
  label: Leadspace Enrichment API
  slug: leadspace-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-enrichment-openapi.yml
- filename: leadspace-discovery-openapi.yml
  format: yaml
  label: Leadspace Discovery API
  slug: leadspace-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-discovery-openapi.yml
- filename: leadspace-intent-openapi.yml
  format: yaml
  label: Leadspace Intent Only API
  slug: leadspace-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-intent-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Leadspace Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Leadspace secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Leadspace
provider_slug: leadspace
scheme_count: 2
schemes:
- description: Perpetual token issued by Leadspace at program setup. Used directly as a bearer credential on every enrichment, discovery, and intent request.
  format: 'Authorization: Bearer API_KEY'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/leadspace-enrichment-openapi.yml
  - openapi/leadspace-discovery-openapi.yml
  - openapi/leadspace-intent-openapi.yml
  type: http
- audience: API_GATEWAY
  description: Username-password (resource owner password credentials) flow. POST the Program ID as `user`, the authentication secret as `pass`, and the audience `API_GATEWAY` to the authorize endpoint to receive a bearer token plus a refreshToken. Tokens expire every 24 hours; refresh with a PUT to the same endpoint.
  flow: password
  name: oauth2
  refreshUrl: https://apigw.leadspace.com/oauth/authorize
  scopes: []
  scopes_note: Leadspace does not document an OAuth scope surface; entitlement is bound to the Program ID rather than to per-request scopes.
  sources:
  - https://support.leadspace.com/hc/en-us/articles/360000827409-API-v4-OAuth-2-0-Diagram
  tokenUrl: https://apigw.leadspace.com/oauth/authorize
  token_ttl_seconds: 86400
  type: oauth2
slug: leadspace-authentication
source_filename: leadspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://support.leadspace.com/hc/en-us/articles/23687993264284-Leadspace-Single-Direct-API-v4-Technical-Specifications\ndocs: https://support.leadspace.com/hc/en-us/articles/360000827409-API-v4-OAuth-2-0-Diagram\nsummary:\n  types:\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - password\n  transport: https-only\n  credential_delivery: >-\n    Leadspace issues a Program ID (username) and an authentication secret / API\n    key out of band, by email, at program setup. A customer may hold multiple\n    API keys, one per program.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: \"Authorization: Bearer API_KEY\"\n    description: >-\n      Perpetual token issued by Leadspace at program setup. Used directly as a\n      bearer credential on every enrichment, discovery, and intent request.\n    sources:\n      - openapi/leadspace-enrichment-openapi.yml\n\
  \      - openapi/leadspace-discovery-openapi.yml\n      - openapi/leadspace-intent-openapi.yml\n  - name: oauth2\n    type: oauth2\n    flow: password\n    description: >-\n      Username-password (resource owner password credentials) flow. POST the\n      Program ID as `user`, the authentication secret as `pass`, and the\n      audience `API_GATEWAY` to the authorize endpoint to receive a bearer\n      token plus a refreshToken. Tokens expire every 24 hours; refresh with a\n      PUT to the same endpoint.\n    tokenUrl: https://apigw.leadspace.com/oauth/authorize\n    refreshUrl: https://apigw.leadspace.com/oauth/authorize\n    token_ttl_seconds: 86400\n    audience: API_GATEWAY\n    scopes: []\n    scopes_note: >-\n      Leadspace does not document an OAuth scope surface; entitlement is bound\n      to the Program ID rather than to per-request scopes.\n    sources:\n      - https://support.leadspace.com/hc/en-us/articles/360000827409-API-v4-OAuth-2-0-Diagram\ntoken_rotation:\n  perpetual_token:\
  \ true\n  recommended_rotation_months: 6\n  hard_expiry_years: 2\n  process: >-\n    Leadspace recommends rotating the perpetual token every six months from the\n    end of the integration period. An unrotated token expires two years after\n    issue. Leadspace generates the replacement, notifies the customer ahead of\n    the end of the token lifecycle (10 working days' notice per the Discovery\n    API docs), and deprecates the old token once migration is confirmed.\nfailure_modes:\n  - status: 401\n    meaning: Wrong credentials, or credentials have expired\n  - status: 403\n    meaning: Program ID is invalid (Discovery API)\n  - status: 427\n    meaning: Insufficient credits, or the program ID is invalid\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/authentication/leadspace-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- B2B Data
- Customer Data Platform
- Data Enrichment
- Intent Data
- Sales Intelligence
- Account-Based Marketing
- Identity Resolution
- Firmographics
- Lead Scoring
- Company
---
