---
api_key_in:
- header
- query
api_specs:
- filename: xoserve-shipper-api-openapi.yml
  format: yaml
  label: Xoserve Shipper API
  slug: xoserve-shipper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-shipper-api-openapi.yml
- filename: xoserve-supplier-api-openapi.yml
  format: yaml
  label: Xoserve Supplier API
  slug: xoserve-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-supplier-api-openapi.yml
- filename: xoserve-meter-asset-api-v1-openapi.yml
  format: yaml
  label: Xoserve Meter Asset API v1
  slug: xoserve-meter-asset-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-meter-asset-api-v1-openapi.yml
- filename: xoserve-meter-asset-api-v2-openapi.yml
  format: yaml
  label: Xoserve Meter Asset API v2
  slug: xoserve-meter-asset-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-meter-asset-api-v2-openapi.yml
auth_types:
- apiKey
description: 'A single auth model across the whole estate: an Azure API Management subscription key, passed either as the `APIKey` request header or as a `subscription-key` query parameter, over HTTPS only. There is no OAuth 2.0, no OpenID Connect, no mTLS and no consumer-consent grant of any kind — the portal reports empty oAuth2AuthenticationSettings and empty openidAuthenticationSettings for all four APIs, and /.well-known/openid-configuration returns 404 on every host. Prefer the header form so the secret does not leak into logs, referrers or browser history.'
kind: authentication
layout: security
method: searched
name: Xoserve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xoserve secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Xoserve
provider_slug: xoserve
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: APIKey
  preferred: true
  sources:
  - openapi/xoserve-meter-asset-api-v1-openapi.yml
  - openapi/xoserve-meter-asset-api-v2-openapi.yml
  - openapi/xoserve-shipper-api-openapi.yml
  - openapi/xoserve-supplier-api-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  preferred: false
  sources:
  - openapi/xoserve-meter-asset-api-v1-openapi.yml
  - openapi/xoserve-meter-asset-api-v2-openapi.yml
  - openapi/xoserve-shipper-api-openapi.yml
  - openapi/xoserve-supplier-api-openapi.yml
  type: apiKey
slug: xoserve-authentication
source_filename: xoserve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Derived from openapi/xoserve-meter-asset-api-v1-openapi.yml,\n  openapi/xoserve-meter-asset-api-v2-openapi.yml, openapi/xoserve-shipper-api-openapi.yml,\n  openapi/xoserve-supplier-api-openapi.yml, then upgraded from the provider's own surfaces:\n  https://discoveryapiportal.correla.com/developer/apis?api-version=2022-04-01-preview\n  (subscriptionKeyParameterNames + authenticationSettings), the live WWW-Authenticate challenge on\n  https://discoveryapi.correla.com (2026-07-27),\n  https://www.xoserve.com/products-services/data-products/gas-apis/ and the Xoserve Try Before You Buy\n  API Service Subscription Guide.\ndocs: https://www.xoserve.com/products-services/data-products/gas-apis/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\ndescription: >-\n  A single auth model across the whole estate: an Azure API Management subscription\
  \ key, passed either\n  as the `APIKey` request header or as a `subscription-key` query parameter, over HTTPS only. There is\n  no OAuth 2.0, no OpenID Connect, no mTLS and no consumer-consent grant of any kind — the portal\n  reports empty oAuth2AuthenticationSettings and empty openidAuthenticationSettings for all four APIs,\n  and /.well-known/openid-configuration returns 404 on every host. Prefer the header form so the\n  secret does not leak into logs, referrers or browser history.\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: APIKey\n  preferred: true\n  sources:\n  - openapi/xoserve-meter-asset-api-v1-openapi.yml\n  - openapi/xoserve-meter-asset-api-v2-openapi.yml\n  - openapi/xoserve-shipper-api-openapi.yml\n  - openapi/xoserve-supplier-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  preferred: false\n  sources:\n  - openapi/xoserve-meter-asset-api-v1-openapi.yml\n  - openapi/xoserve-meter-asset-api-v2-openapi.yml\n\
  \  - openapi/xoserve-shipper-api-openapi.yml\n  - openapi/xoserve-supplier-api-openapi.yml\nchallenge:\n  status: 401\n  header: 'WWW-Authenticate: AzureApiManagementKey realm=\"https://discoveryapi.correla.com/<api>\",name=\"APIKey\",type=\"header\"'\n  observed: '2026-07-27'\nkey_model:\n  issuer: Xoserve (via Correla-operated Azure API Management)\n  scope: >-\n    One key per subscription. The provider's subscription guide states the APIKey \"is associated with\n    each created subscription and cannot be utilized for any other subscriptions.\" An Application\n    Secret is displayed alongside the key but is explicitly not required.\n  scopes: none — the API declares no OAuth scopes and no per-operation permission model\n  rotation: not documented\n  expiry: not documented\n  transport: HTTPS only (portal reports protocols [\"https\"])\naccess_gate:\n  self_serve: false\n  subscription_required: true\n  approval_required: true\n  routes:\n  - product: Supply Point Quantities (Shipper\
  \ API)\n    eligibility: Licensed GB gas Shippers only\n    apply_to: xoserve.customer.lifecycle.team@xoserve.co.uk\n    issuance: Access details provided after the subscription contract is countersigned.\n  - product: Supply Point Enquiry (Supplier API)\n    eligibility: REC parties, subject to the REC Data Access Matrix\n    apply_to: enquiries@recmanager.co.uk (Retail Energy Code Company)\n    administration: REC Portal (https://recportal.co.uk/), including an annual GES password reset process\n  - product: Meter Asset Enquiry (Meter Asset v1/v2)\n    eligibility: REC parties, subject to the REC Data Access Matrix\n    apply_to: enquiries@recmanager.co.uk (Retail Energy Code Company)\n    administration: REC Portal (https://recportal.co.uk/)\n  trial:\n    name: Try Before You Buy\n    login: SAP S-User ID issued by Xoserve\n    detail: sandbox/xoserve-sandbox.yml\nnotes: >-\n  Browsing is open, calling is not: the portal catalogue, product descriptions and OpenAPI exports are\n  all\
  \ reachable anonymously, but there is no self-serve signup that ends in a working key. Because a\n  key is long-lived, unscoped and carries no expiry signal, it must never be handed to a model or\n  embedded client-side — see agentic-access/xoserve-agentic-access.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/authentication/xoserve-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Energy
- United Kingdom
- Gas
- Utilities
- Energy Markets
- Meter Data
- Gas Networks
- Central Data Service Provider
- Data Services
---
