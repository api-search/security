---
api_key_in: []
api_specs:
- filename: nuvemshop-tiendanube-events-asyncapi.yml
  format: yaml
  label: Nuvemshop Tiendanube API
  slug: nuvemshop-tiendanube-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvemshop-tiendanube/refs/heads/main/asyncapi/nuvemshop-tiendanube-events-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nuvemshop Tiendanube Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nuvemshop Tiendanube secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nuvemshop Tiendanube
provider_slug: nuvemshop-tiendanube
scheme_count: 1
schemes:
- description: Restricted form of OAuth 2 supporting only the authorization_code grant. Access tokens are bearer tokens that do not expire, but are invalidated when a new token is issued or the app is uninstalled.
  flows:
  - alt_domain: nuvemshop.com.br
    authorizationUrl: https://www.tiendanube.com/apps/{app_id}/authorize
    flow: authorizationCode
    notes: Authorization code expires after 5 minutes. Token request POSTs a JSON body with client_id, client_secret, grant_type=authorization_code and code. Token response returns access_token, token_type=bearer, scope and user_id (the store id).
    tokenUrl: https://www.tiendanube.com/apps/authorize/token
  name: OAuth2
  type: oauth2
slug: nuvemshop-tiendanube-authentication
source_filename: nuvemshop-tiendanube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://tiendanube.github.io/api-documentation/authentication\ndocs: https://tiendanube.github.io/api-documentation/authentication\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  token_transport: bearer\n  token_expiry: none\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Restricted form of OAuth 2 supporting only the authorization_code grant.\n    Access tokens are bearer tokens that do not expire, but are invalidated when\n    a new token is issued or the app is uninstalled.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.tiendanube.com/apps/{app_id}/authorize\n    tokenUrl: https://www.tiendanube.com/apps/authorize/token\n    alt_domain: nuvemshop.com.br\n    notes: >-\n      Authorization code expires after 5 minutes. Token request POSTs a JSON body\n      with client_id, client_secret, grant_type=authorization_code and code.\n      Token\
  \ response returns access_token, token_type=bearer, scope and user_id\n      (the store id).\nrequest_auth:\n  header: 'Authorization: bearer <access_token>'\n  user_agent_required: true\n  user_agent_format: 'AppName (email@example.com) or AppName (https://website.com)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvemshop-tiendanube/refs/heads/main/authentication/nuvemshop-tiendanube-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- E-Commerce
- Retail
- Online Stores
- Payments
- Shipping
- Webhooks
- OAuth
- Latin America
- Storefront
- Apps Platform
---
