---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Shopline Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SHOPLINE secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SHOPLINE
provider_slug: shopline
scheme_count: 2
schemes:
- access_token:
    format: JWT
    lifetime: 10 hours
    refresh: Refresh Token interface; original token remains valid 5 minutes after refresh
    revoke: Cancel Authorization interface (token invalidated immediately)
    transport: 'Authorization: Bearer <accessToken>'
  app_credentials:
  - App Key
  - App Secret
  callback: After the merchant grants permissions during OAuth, SHOPLINE redirects to the app Callback URL with a temporary OAuth code, which the app exchanges for an accessToken.
  docs: https://developer.shopline.com/docs/apps/application-management/creating-an-app
  flow: authorizationCode
  grant: authorization_code
  name: OAuth2 (Custom and Public apps)
  obtained_in: SHOPLINE Developer Center
  scopes_model: The accessToken carries the scopes the app requested at install time (read_* / write_* permissions, e.g. read_bulkoperation, write_bulkoperation).
  type: oauth2
- docs: https://developer.shopline.com/docs/apps/application-management/application-distribution-methods
  in: header
  lifetime: 3 years (email reminder before expiry)
  limitations: Cannot use App Bridge or App Extensions
  name: Private app token
  parameter_name: Authorization
  refresh: Refreshed from within the store admin; original token valid 30 minutes after refresh
  revoke: Delete the app in the store admin (token invalidated)
  scheme_note: Bearer JWT minted in the store admin backend
  type: apiKey
slug: shopline-authentication
source_filename: shopline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.shopline.com/docs/apps/api-instructions-for-use/rest-admin-api/overview\ndocs: https://developer.shopline.com/docs/apps/api-instructions-for-use/rest-admin-api/overview\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  token_transport: \"Authorization: Bearer <accessToken> (JWT)\"\nnotes: >-\n  SHOPLINE Open Platform gates all API access behind Store Authorization, which\n  differs by app distribution method. Custom apps and Public apps use OAuth 2.0\n  (authorization-code); Private apps use a long-lived token minted in the store\n  admin. Access tokens are JWTs passed in the Authorization header using the\n  Bearer scheme. No downloadable OpenAPI/Swagger security scheme was published,\n  so this profile is captured from the developer documentation rather than\n  derived from a spec.\nschemes:\n  - name: OAuth2 (Custom and Public apps)\n    type: oauth2\n\
  \    flow: authorizationCode\n    grant: authorization_code\n    app_credentials: [App Key, App Secret]\n    obtained_in: SHOPLINE Developer Center\n    callback: >-\n      After the merchant grants permissions during OAuth, SHOPLINE redirects to\n      the app Callback URL with a temporary OAuth code, which the app exchanges\n      for an accessToken.\n    access_token:\n      format: JWT\n      transport: \"Authorization: Bearer <accessToken>\"\n      lifetime: 10 hours\n      refresh: Refresh Token interface; original token remains valid 5 minutes after refresh\n      revoke: Cancel Authorization interface (token invalidated immediately)\n    scopes_model: >-\n      The accessToken carries the scopes the app requested at install time\n      (read_* / write_* permissions, e.g. read_bulkoperation, write_bulkoperation).\n    docs: https://developer.shopline.com/docs/apps/application-management/creating-an-app\n  - name: Private app token\n    type: apiKey\n    in: header\n    parameter_name:\
  \ Authorization\n    scheme_note: Bearer JWT minted in the store admin backend\n    lifetime: 3 years (email reminder before expiry)\n    refresh: Refreshed from within the store admin; original token valid 30 minutes after refresh\n    revoke: Delete the app in the store admin (token invalidated)\n    limitations: Cannot use App Bridge or App Extensions\n    docs: https://developer.shopline.com/docs/apps/application-management/application-distribution-methods\nrequest_headers:\n  Authorization: \"Bearer <accessToken>\"\n  Content-Type: \"application/json; charset=utf-8\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopline/refs/heads/main/authentication/shopline-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- E-Commerce
- Commerce
- Retail
- Point of Sale
- Storefront
- Payments
- Webhooks
- GraphQL
- Developer Platform
- Apps
---
