---
api_key_in:
- header
api_specs:
- filename: shoplazza-access-api-openapi.yml
  format: yaml
  label: Shoplazza Access API
  slug: shoplazza-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-access-api-openapi.yml
- filename: shoplazza-app-proxy-api-openapi.yml
  format: yaml
  label: Shoplazza App Proxy API
  slug: shoplazza-app-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-app-proxy-api-openapi.yml
- filename: shoplazza-billing-api-api-openapi.yml
  format: yaml
  label: Shoplazza Billing API API
  slug: shoplazza-billing-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-billing-api-api-openapi.yml
- filename: shoplazza-custom-area-api-openapi.yml
  format: yaml
  label: Shoplazza Custom Area API
  slug: shoplazza-custom-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-custom-area-api-openapi.yml
- filename: shoplazza-customer-api-openapi.yml
  format: yaml
  label: Shoplazza Customer API
  slug: shoplazza-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-customer-api-openapi.yml
- filename: shoplazza-data-api-openapi.yml
  format: yaml
  label: Shoplazza Data API
  slug: shoplazza-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-data-api-openapi.yml
- filename: shoplazza-discounts-api-openapi.yml
  format: yaml
  label: Shoplazza Discounts API
  slug: shoplazza-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-discounts-api-openapi.yml
- filename: shoplazza-file-api-openapi.yml
  format: yaml
  label: Shoplazza File API
  slug: shoplazza-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-file-api-openapi.yml
- filename: shoplazza-fullfillment-api-openapi.yml
  format: yaml
  label: Shoplazza Fullfillment API
  slug: shoplazza-fullfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-fullfillment-api-openapi.yml
- filename: shoplazza-gift-card-api-openapi.yml
  format: yaml
  label: Shoplazza Gift Card API
  slug: shoplazza-gift-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-gift-card-api-openapi.yml
- filename: shoplazza-meta-definition-api-openapi.yml
  format: yaml
  label: Shoplazza Meta Definition API
  slug: shoplazza-meta-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-meta-definition-api-openapi.yml
- filename: shoplazza-metafield-api-openapi.yml
  format: yaml
  label: Shoplazza Metafield API
  slug: shoplazza-metafield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-metafield-api-openapi.yml
- filename: shoplazza-order-api-openapi.yml
  format: yaml
  label: Shoplazza Order API
  slug: shoplazza-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-order-api-openapi.yml
- filename: shoplazza-order-risk-api-openapi.yml
  format: yaml
  label: Shoplazza Order Risk API
  slug: shoplazza-order-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-order-risk-api-openapi.yml
- filename: shoplazza-page-api-openapi.yml
  format: yaml
  label: Shoplazza Page API
  slug: shoplazza-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-page-api-openapi.yml
- filename: shoplazza-product-api-openapi.yml
  format: yaml
  label: Shoplazza Product API
  slug: shoplazza-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-product-api-openapi.yml
- filename: shoplazza-redirect-api-openapi.yml
  format: yaml
  label: Shoplazza Redirect API
  slug: shoplazza-redirect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-redirect-api-openapi.yml
- filename: shoplazza-shop-api-openapi.yml
  format: yaml
  label: Shoplazza Shop API
  slug: shoplazza-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-shop-api-openapi.yml
- filename: shoplazza-theme-api-openapi.yml
  format: yaml
  label: Shoplazza Theme API
  slug: shoplazza-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-theme-api-openapi.yml
- filename: shoplazza-webhook-api-openapi.yml
  format: yaml
  label: Shoplazza Webhook API
  slug: shoplazza-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-webhook-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Shoplazza Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Shoplazza secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Shoplazza
provider_slug: shoplazza
scheme_count: 2
schemes:
- description: Public apps request access scopes from the merchant during installation and exchange an authorization code for an access token + refresh token. Token is then presented as the access-token header on Admin API calls.
  flow: authorizationCode
  name: OAuth2 (authorization code)
  scopes_ref: scopes/shoplazza-scopes.yml
  source: docs
  type: oauth2
- description: The OAuth-issued access token is presented on every Admin API request via the access-token HTTP header (declared as the operation-level security scheme in the OpenAPI spec).
  in: header
  name: apikey-header-access-token
  parameter_name: access-token
  sources:
  - openapi/shoplazza-admin-openapi-original.json
  type: apiKey
slug: shoplazza-authentication
source_filename: shoplazza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.shoplazza.dev/docs/app/building-blocks/authentication/\ndocs: https://www.shoplazza.dev/docs/app/building-blocks/authentication/\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  api_key_name: access-token\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Shoplazza uses OAuth 2.0 (authorization code grant) to authorize third-party\n    public apps. The app receives an access token (with refresh token) that is\n    sent on every Admin API request in the access-token request header. OAuth\n    callbacks and webhooks are additionally verified with an HMAC signature.\n    App Bridge embedded apps use short-lived session tokens.\nschemes:\n- name: OAuth2 (authorization code)\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    Public apps request access scopes from the merchant during installation and\n    exchange an authorization code for an access token + refresh token. Token is\n\
  \    then presented as the access-token header on Admin API calls.\n  scopes_ref: scopes/shoplazza-scopes.yml\n  source: docs\n- name: apikey-header-access-token\n  type: apiKey\n  in: header\n  parameter_name: access-token\n  description: >-\n    The OAuth-issued access token is presented on every Admin API request via\n    the access-token HTTP header (declared as the operation-level security\n    scheme in the OpenAPI spec).\n  sources: [openapi/shoplazza-admin-openapi-original.json]\nsignature_verification:\n  method: HMAC\n  applies_to: [oauth-callbacks, webhooks]\n  docs: https://www.shoplazza.dev/docs/app/building-blocks/authentication/\nembedded_session_tokens:\n  used_by: App Bridge\n  docs: https://www.shoplazza.dev/docs/app/developer-tools/app-bridge/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/authentication/shoplazza-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Enterprise
- E-Commerce
- Online Store
- Retail
- Payments
- Webhook
- REST API
- Application
- Developer Platform
---
