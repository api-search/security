---
api_key_in: []
api_specs:
- filename: paack-api-systems
  format: yaml
  label: Paack API
  slug: paack-api
  spec_type: Postman
  url: https://www.postman.com/paacklogistics/paack-apis/collection/p93tvmy/paack-api-systems
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Paack Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Paack secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Paack
provider_slug: paack
scheme_count: 1
schemes:
- flow: clientCredentials
  identity_provider: Auth0
  name: OAuth2ClientCredentials
  parameters:
  - client_id
  - client_secret
  - grant_type
  - audience
  request_content_type: application/json
  response_fields:
  - access_token
  - expires_in
  - token_type
  token_ttl_seconds: 86400
  token_url_production: https://paack-hq-production.eu.auth0.com/oauth/token
  token_url_staging: https://paack-hq-staging.eu.auth0.com/oauth/token
  type: oauth2
  usage: 'Send the access_token as `Authorization: Bearer <access_token>` on every API request.'
slug: paack-authentication
source_filename: paack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://paack.readme.io/docs/start-auth\ndocs: https://paack.readme.io/reference/token\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_format: JWT\n  token_type: Bearer\n  token_ttl_seconds: 86400\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  identity_provider: Auth0\n  token_url_production: https://paack-hq-production.eu.auth0.com/oauth/token\n  token_url_staging: https://paack-hq-staging.eu.auth0.com/oauth/token\n  request_content_type: application/json\n  parameters:\n  - client_id        # issued by Paack Customer Solutions team\n  - client_secret    # issued by Paack Customer Solutions team\n  - grant_type       # fixed value: client_credentials\n  - audience         # https://ggl-pro-gcp-gw (prod) / https://ggl-stg-gcp-gw (staging)\n  response_fields: [access_token, expires_in, token_type]\n  usage: 'Send the access_token as `Authorization: Bearer <access_token>`\
  \ on every API request.'\n  token_ttl_seconds: 86400\nnotes: >-\n  Credentials (client_id / client_secret) are provisioned by Paack's Customer\n  Solutions team. The same OAuth2 client-credentials flow is used for staging and\n  production, differentiated by the token URL and the audience value.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/authentication/paack-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Logistics
- Last Mile Delivery
- Parcel Delivery
- E-commerce
- Shipping
- Fulfillment
- Tracking
- Reverse Logistics
---
