---
api_key_in:
- query
api_specs:
- filename: skimbit-merchant-openapi.yml
  format: yaml
  label: Skimlinks Merchant API
  slug: skimlinks-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-merchant-openapi.yml
- filename: skimbit-reporting-openapi.yml
  format: yaml
  label: Skimlinks Reporting API
  slug: skimlinks-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-reporting-openapi.yml
- filename: skimbit-product-key-openapi.yml
  format: yaml
  label: Skimlinks Product Key API
  slug: skimlinks-product-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-product-key-openapi.yml
auth_types:
- apiKey
- oauth2-like-client-credentials
description: ''
kind: authentication
layout: security
method: searched
name: Skimbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: SkimBit secures its APIs with apiKey and oauth2-like-client-credentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SkimBit
provider_slug: skimbit
scheme_count: 1
schemes:
- description: Timestamp-based access token obtained from https://authentication.skimapis.com/access_token via a client_credentials grant using your client_id and client_secret. Passed as the access_token query parameter on every request.
  in: query
  name: access_token
  parameter: access_token
  sources:
  - openapi/skimbit-merchant-openapi.yml
  - openapi/skimbit-product-key-openapi.yml
  - openapi/skimbit-reporting-openapi.yml
  type: apiKey
slug: skimbit-authentication
source_filename: skimbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  openapi/skimbit-merchant-openapi.yml, openapi/skimbit-reporting-openapi.yml,\n  openapi/skimbit-product-key-openapi.yml, and the developer docs at\n  https://developers.skimlinks.com/merchant.html\ndocs: https://hub.skimlinks.com/toolbox/api#credentials\nsummary:\n  types:\n  - apiKey\n  - oauth2-like-client-credentials\n  api_key_in:\n  - query\n  model: >-\n    Two-step, timestamp-based access token. Publishers retrieve a Client ID and\n    Client Secret from the Publisher Hub (Toolbox > APIs > API Authentication\n    credentials), exchange them for a short-lived access_token at the\n    authentication API, then pass that access_token as a query parameter on\n    every Merchant/Reporting/Product Key request.\ntoken_endpoint:\n  url: https://authentication.skimapis.com/access_token\n  method: POST\n  content_type: application/json\n  grant_type: client_credentials\n  request_fields: [client_id, client_secret, grant_type]\n\
  \  response_fields: [access_token, timestamp, expiry_timestamp]\n  token_ttl_seconds: 604800\n  note: >-\n    The access_token is a timestamp-based value of the form\n    \"<id>:<timestamp>:<hash>\". expiry_timestamp is returned with each token; in\n    the documented example the token is valid for ~7 days. The Product Key API\n    requires a separate, dedicated Client ID / Client Secret issued on request.\nschemes:\n- name: access_token\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: >-\n    Timestamp-based access token obtained from\n    https://authentication.skimapis.com/access_token via a client_credentials\n    grant using your client_id and client_secret. Passed as the access_token\n    query parameter on every request.\n  sources:\n  - openapi/skimbit-merchant-openapi.yml\n  - openapi/skimbit-product-key-openapi.yml\n  - openapi/skimbit-reporting-openapi.yml\nlegacy:\n  name: apikey (v3)\n  description: >-\n    The deprecated v3 Merchant API endpoints authenticate\
  \ with a public apikey\n    plus account_type and account_id query parameters instead of an\n    access_token. Superseded by the v4 access_token flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/authentication/skimbit-authentication.yml
summary_line: apiKey/oauth2-like-client-credentials · 1 scheme
tags:
- Company
- Affiliate Marketing
- Content Monetization
- Commerce
- Publishers
- Advertising
- Retail
- Reporting
- Products
- eCommerce
---
