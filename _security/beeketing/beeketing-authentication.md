---
api_key_in:
- query
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Beeketing Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Beeketing secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Beeketing
provider_slug: beeketing
scheme_count: 2
schemes:
- app_type: public
  authorizationUrl: https://{shop}.onshopbase.com/admin/oauth/authorize
  client_credentials: API key + API secret key issued in the Partner Dashboard
  docs: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication/oauth.md
  install_verification: HMAC signature on install/redirect requests
  name: PublicAppOAuth2
  scheme: authorizationCode
  scope_param: comma-separated scopes (e.g. write_orders,read_customers)
  tokenUrl: https://{shop}.onshopbase.com/admin/oauth/access_token.json
  type: oauth2
- app_type: private
  description: Private apps interact with the API on behalf of a single store using HTTP Basic authentication; credentials are generated from that store's admin.
  docs: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication/private-apps.md
  name: PrivateAppBasic
  scheme: basic
  type: http
slug: beeketing-authentication
source_filename: beeketing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication.md\ndocs: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication.md\nsummary:\n  types: [oauth2, http]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    ShopBase supports two app types. Public apps authenticate via OAuth 2.0\n    authorization-code grant (API key + secret from the Partner Dashboard,\n    per-store access token). Private apps authenticate via HTTP Basic\n    authentication with credentials generated in the store admin.\nschemes:\n- name: PublicAppOAuth2\n  type: oauth2\n  app_type: public\n  scheme: authorizationCode\n  authorizationUrl: https://{shop}.onshopbase.com/admin/oauth/authorize\n  tokenUrl: https://{shop}.onshopbase.com/admin/oauth/access_token.json\n  client_credentials: API key + API secret key issued in the Partner Dashboard\n  install_verification: HMAC\
  \ signature on install/redirect requests\n  scope_param: comma-separated scopes (e.g. write_orders,read_customers)\n  docs: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication/oauth.md\n- name: PrivateAppBasic\n  type: http\n  app_type: private\n  scheme: basic\n  description: >-\n    Private apps interact with the API on behalf of a single store using HTTP\n    Basic authentication; credentials are generated from that store's admin.\n  docs: https://developers.shopbase.com/build-an-app/making-your-first-request/authentication/private-apps.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeketing/refs/heads/main/authentication/beeketing-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- E-commerce
- Cross-border Commerce
- Marketing
- Shopify Apps
- REST API
- OAuth
- Webhooks
- Themes
- Payments
---
