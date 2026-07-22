---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Meal Ticket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meal Ticket secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Meal Ticket
provider_slug: meal-ticket
scheme_count: 1
schemes:
- authorization_endpoint: https://login.mealticket.com/authorize
  id_token_signing_alg:
  - RS256
  issuer: https://login.mealticket.com/
  jwks_uri: https://login.mealticket.com/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://login.mealticket.com/.well-known/openid-configuration
  response_types:
  - code
  scopes:
  - openid
  - email
  sources:
  - well-known/meal-ticket-openid-configuration.json
  token_endpoint: https://login.mealticket.com/auth/token
  type: openIdConnect
slug: meal-ticket-authentication
source_filename: meal-ticket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://login.mealticket.com/.well-known/openid-configuration\nsummary:\n  types: [openIdConnect]\n  surface: customer-login-sso\n  note: >-\n    Meal Ticket exposes an OpenID Connect provider for its customer / product\n    login (login.mealticket.com). No public developer API or API-key/OAuth\n    developer program is documented, so this profile captures the identity/SSO\n    surface only.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://login.mealticket.com/.well-known/openid-configuration\n  issuer: https://login.mealticket.com/\n  authorization_endpoint: https://login.mealticket.com/authorize\n  token_endpoint: https://login.mealticket.com/auth/token\n  jwks_uri: https://login.mealticket.com/.well-known/jwks.json\n  response_types: [code]\n  id_token_signing_alg: [RS256]\n  scopes: [openid, email]\n  sources: [well-known/meal-ticket-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meal-ticket/refs/heads/main/authentication/meal-ticket-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Foodservice
- Foodservice Distribution
- Restaurants
- Rebate Management
- Profitability Management
- Supply Chain
- SaaS
---
