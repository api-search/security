---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Banyan Systems Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Banyan Systems secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Banyan Systems
provider_slug: banyan-systems
scheme_count: 1
schemes:
- credentials: Client ID and Client Secret issued by a Banyan representative during onboarding
  flow: clientCredentials
  issuer: https://api.banyan.com
  name: OAuth2ClientCredentials
  request:
    content_type: application/x-www-form-urlencoded
    grant_type: client_credentials
    parameters:
    - client_id
    - client_secret
  sources:
  - https://developers.banyan.com/reference/oauth-token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  token_expiry: Tokens expire after 60 minutes; an expired token returns HTTP 401, re-call /oauth/token for a fresh one
  token_url: https://api.banyan.com/oauth/token
  type: oauth2
  usage_header: 'Authorization: Bearer {access_token}'
slug: banyan-systems-authentication
source_filename: banyan-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.banyan.com/docs/banyan-authentication\ndocs: https://developers.banyan.com/docs/banyan-authentication\nwell_known: https://api.banyan.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  token_type: bearer\n  token_ttl_seconds: 3600\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.banyan.com/oauth/token\n  issuer: https://api.banyan.com\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  credentials: Client ID and Client Secret issued by a Banyan representative during onboarding\n  request:\n    content_type: application/x-www-form-urlencoded\n    parameters:\n    - client_id\n    - client_secret\n    grant_type: client_credentials\n  usage_header: 'Authorization: Bearer {access_token}'\n  token_expiry: Tokens expire after\
  \ 60 minutes; an expired token returns HTTP 401, re-call /oauth/token for a fresh one\n  sources:\n  - https://developers.banyan.com/reference/oauth-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/authentication/banyan-systems-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Receipt Data
- Transaction Enrichment
- Item-Level Data
- Card-Linked Offers
- Fintech
- Payments
- Data Collaboration
- Webhooks
---
