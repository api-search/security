---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cleartax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cleartax secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cleartax
provider_slug: cleartax
scheme_count: 2
schemes:
- description: API client secret generated from the Clear UI, sent to the Generate Access Token API (GET /integration/v1/authz/token) to obtain an access token. Must not be empty.
  in: header
  name: clientSecret
  parameter: x-clear-client-secret
  type: apiKey
- description: Access token obtained from the token endpoint, sent in the request header of any product API (CFC, GST, Max ITC, E-Invoicing, Invoicing).
  in: header
  name: accessToken
  parameter: x-cleartax-auth-token
  type: apiKey
slug: cleartax-authentication
source_filename: cleartax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cleartax.in/cleartax-docs/clear-finance-cloud/learn-clear-finance-cloud-basics/access-token\ndocs:\n- https://docs.cleartax.in/cleartax-docs/clear-finance-cloud/learn-clear-finance-cloud-basics/access-token\n- https://docs.cleartax.in/cleartax-docs/clear-finance-cloud/cfc-api-reference/generate-access-token-api\n- https://docs.cleartax.in/cleartax-docs/e-invoicing-api/learn-e-invoicing-api-basics/how-to-get-e-invoicing-user-auth-token\nsummary:\n  types:\n  - apiKey\n  model: >-\n    Client-secret exchanged for a bearer access token. The API client secret is generated\n    in the Clear UI and passed to the token endpoint to mint a short-lived access token,\n    which is then sent on every product API request. Access tokens can be regenerated and\n    revoked; generating a new token invalidates the previous one.\nschemes:\n- name: clientSecret\n  type: apiKey\n  in: header\n  parameter: x-clear-client-secret\n \
  \ description: >-\n    API client secret generated from the Clear UI, sent to the Generate Access Token API\n    (GET /integration/v1/authz/token) to obtain an access token. Must not be empty.\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: x-cleartax-auth-token\n  description: >-\n    Access token obtained from the token endpoint, sent in the request header of any\n    product API (CFC, GST, Max ITC, E-Invoicing, Invoicing).\ntoken_endpoint:\n  method: GET\n  path: /integration/v1/authz/token\n  sandbox_url: https://api-sandbox.clear.in/integration/v1/authz/token\n  production_url: https://api.clear.in/integration/v1/authz/token\nnotes: >-\n  The E-Invoicing/E-Waybill product additionally uses a per-GSTIN user auth token layered\n  on the Clear access token; base URL varies by region (India vs KSA) and environment\n  (sandbox vs production).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleartax/refs/heads/main/authentication/cleartax-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Tax
- GST
- E-Invoicing
- Compliance
- Fintech
- Accounting
- India
- Financial Automation
- Government
---
