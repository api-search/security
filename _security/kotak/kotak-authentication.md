---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kotak Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kotak Mahindra Bank secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kotak Mahindra Bank
provider_slug: kotak
scheme_count: 1
schemes:
- authorization_url: null
  catalog_category: authorization-services
  catalog_code: authorization-services-o-auth
  description: This API call will provide access token required to invoke various API offerings.
  name: OAuth 2.0
  scopes_published: false
  source: https://api.kotak.bank.in/mapping/
  token_url: null
  type: oauth2
slug: kotak-authentication
source_filename: kotak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.kotak.bank.in/mapping/\ndocs: https://api.kotak.bank.in/explore\nnotes: >-\n  Derived from the Kotak API Platform's own published catalog rather than from an\n  OpenAPI document — Kotak publishes no public specification (specs are released\n  to registered developers after login), so the mechanical\n  derive-authentication.py pass had nothing to read. The catalog does declare\n  authentication as a first-class product category: \"Authorization services\"\n  contains an \"O-auth 2.0\" API whose published description is \"This API call will\n  provide access token required to invoke various API offerings.\" Token endpoint\n  URL, grant type, and scope list are not published publicly and are NOT recorded\n  here.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows: []\n  flows_documented: false\nschemes:\n- name: OAuth 2.0\n  type: oauth2\n  catalog_code: authorization-services-o-auth\n  catalog_category: authorization-services\n\
  \  description: >-\n    This API call will provide access token required to invoke various API\n    offerings.\n  source: https://api.kotak.bank.in/mapping/\n  token_url: null\n  authorization_url: null\n  scopes_published: false\ngaps:\n- OAuth 2.0 grant types / flows are not publicly documented\n- token and authorization endpoint URLs are not publicly documented\n- no scope or permission reference is published outside the gated portal\n- no /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotak/refs/heads/main/authentication/kotak-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Banking
- Financial Services
- Open Banking
- Payments
- Collections
- Trade Finance
- Corporate Banking
- India
- UPI
---
