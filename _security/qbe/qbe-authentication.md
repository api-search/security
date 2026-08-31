---
api_key_in:
- header
- query
api_specs:
- filename: qbe-ctp-switch-api-openapi.yml
  format: yaml
  label: QBE Insurance CTP Switch API
  slug: qbe-ctp-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/openapi/qbe-ctp-switch-api-openapi.yml
- filename: qbe-digital-brokers-api-openapi.yml
  format: yaml
  label: QBE Insurance Digital Brokers API
  slug: qbe-digital-brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/openapi/qbe-digital-brokers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Qbe Authentication
name_suffix: Authentication
oauth_flows: []
overview: QBE Insurance secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: QBE Insurance
provider_slug: qbe
scheme_count: 2
schemes:
- description: Azure API Management subscription key. Issued only against an approved subscription to the ANZO Digital Brokers or ANZO CTP Service product (subscriptionRequired true, approvalRequired true, subscriptionsLimit 10).
  in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  region: Australia
  sources:
  - openapi/qbe-anzo-digital-brokers-openapi.yml
  - openapi/qbe-ctp-switch-service-openapi.yml
  type: apiKey
- description: The same APIM subscription key passed as a query-string parameter instead of a header.
  in: query
  name: apiKeyQuery
  parameter: subscription-key
  region: Australia
  sources:
  - openapi/qbe-anzo-digital-brokers-openapi.yml
  - openapi/qbe-ctp-switch-service-openapi.yml
  type: apiKey
slug: qbe-authentication
source_filename: qbe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  openapi/qbe-anzo-digital-brokers-openapi.yml, openapi/qbe-ctp-switch-service-openapi.yml,\n  https://connect.api-au.qbe.com/developer/apis?api-version=2022-04-01-preview (HTTP 200),\n  https://partnerportal-api.qbena.com/guide (HTTP 200)\ndocs: https://connect.api-au.qbe.com/getting-started\nnotes: >-\n  QBE runs two separate, unrelated partner API estates with two different authentication models, and\n  neither is self-serve. Both are Azure API Management fronted, and in both cases credentials are issued\n  by QBE after a business/security approval — there is no signup that yields a working key. No OAuth2 or\n  OpenID Connect is configured on the Australian estate: the APIM authenticationSettings arrays are empty\n  on both published APIs and /.well-known/openid-configuration returns 404 on connect.api-au.qbe.com,\n  gateway.api-au.qbe.com and partnerportal-api.qbena.com. QBE North America does document a token\n  exchange\
  \ (client id + secret -> JWT access token) but publishes no authorization-server metadata.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  self_serve: false\n  approval_required: true\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  region: Australia\n  description: >-\n    Azure API Management subscription key. Issued only against an approved subscription to the ANZO\n    Digital Brokers or ANZO CTP Service product (subscriptionRequired true, approvalRequired true,\n    subscriptionsLimit 10).\n  sources:\n  - openapi/qbe-anzo-digital-brokers-openapi.yml\n  - openapi/qbe-ctp-switch-service-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  region: Australia\n  description: The same APIM subscription key passed as a query-string parameter instead of a header.\n  sources:\n  - openapi/qbe-anzo-digital-brokers-openapi.yml\n  - openapi/qbe-ctp-switch-service-openapi.yml\n\
  additional_credentials:\n  region: Australia\n  api: QBE Australia ANZO Digital Brokers Experience API\n  note: >-\n    The APIM subscription key alone is not sufficient. Every business operation additionally requires\n    per-partner credentials and a partner identity, declared as required headers in QBE's own published\n    operation definitions. These are NOT modelled as OpenAPI securitySchemes by QBE, but they are part of\n    the real auth contract.\n  headers:\n  - name: X-ClientID\n    required: true\n    operations: 13\n    description: Partner client identifier issued by QBE.\n  - name: X-ClientSecret\n    required: true\n    operations: 13\n    description: Partner client secret issued by QBE.\n  - name: X-Partner-Id\n    required: true\n    operations: 12\n    enum: [AUSTBROKERS, MARSH, PSC]\n    description: >-\n      The calling broker partner. Constrained to a fixed enumeration of QBE's named broker groups, which\n      is why this API cannot be consumed by an arbitrary developer\
  \ even with a key.\n  - name: X-TrackingID\n    required: true\n    operations: 14\n    description: Source system's tracking ID for troubleshooting / analysis purposes.\nnorth_america:\n  portal: https://partnerportal-api.qbena.com/\n  guide: https://partnerportal-api.qbena.com/guide\n  probe_status: 200\n  model: token-exchange + subscription key\n  description: >-\n    QBE North America's API Product Hub documents a two-factor call contract: run the portal's `auth`\n    API `partnertoken` operation with the client id and secret QBE emails you to mint a JWT access\n    token, then send that access token together with a QBE-API-Subscription-Key header to the product\n    endpoint. Credentials are sent by the QBE Business team after approval; portal sign-in credentials\n    are emailed and the user is told to change the password immediately. Product subscriptions follow a\n    \"<Partner Name>-<Product Name>\" naming convention and require accepting Terms & Conditions.\n  headers:\n  -\
  \ name: Authorization\n    description: Bearer JWT access token minted by the portal `auth` / `partnertoken` operation.\n  - name: QBE-API-Subscription-Key\n    description: Per-subscription product key found on the portal profile page.\n  token_operation: https://partnerportal-api.qbena.com/api-details#api=auth&operation=partnertoken\n  scopes_published: false\nprobed_and_absent:\n- url: https://connect.api-au.qbe.com/.well-known/openid-configuration\n  status: 404\n- url: https://connect.api-au.qbe.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://connect.api-au.qbe.com/.well-known/oauth-protected-resource\n  status: 404\n- url: https://gateway.api-au.qbe.com/.well-known/openid-configuration\n  status: 404\n- url: https://partnerportal-api.qbena.com/.well-known/openid-configuration\n  status: 404\nrelated:\n  scopes: null\n  conventions: conventions/qbe-conventions.yml\n  well_known: well-known/qbe-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/authentication/qbe-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Insurance
- Australia
- Property and Casualty
- Commercial Insurance
- Underwriting
- Policy Administration
- Quotes
- Brokers
- Reinsurance
- Carrier
- Partner API
---
