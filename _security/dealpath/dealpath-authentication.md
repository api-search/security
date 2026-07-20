---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Dealpath Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dealpath secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dealpath
provider_slug: dealpath
scheme_count: 1
schemes:
- description: 'Authorization: Bearer <token> header on every request. The token is obtained from Dealpath (customer-provisioned); there is no public OAuth authorization endpoint.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://api.dealpath.com/ (401 challenge)
  - https://dealpath.stoplight.io/docs/dealpath-api
  type: http
slug: dealpath-authentication
source_filename: dealpath-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.dealpath.com/ (HTTP 401 challenge) + https://dealpath.stoplight.io/docs/dealpath-api\ndocs: https://dealpath.stoplight.io/docs/dealpath-api\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    The Dealpath API requires a bearer authorization token issued by Dealpath;\n    the live 401 challenge from https://api.dealpath.com/ returns\n    \"No authorization token found in the request header. Please obtain an auth\n    token from Dealpath.\" Tokens are provisioned by Dealpath (not self-service).\n    Note: SSO to the Dealpath application (distinct from API auth) supports\n    Okta, OneLogin, Microsoft Azure and SAML 2.0.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Authorization: Bearer <token> header on every request. The token is obtained\n    from Dealpath (customer-provisioned); there is no public OAuth authorization\n    endpoint.\n  sources:\n\
  \  - https://api.dealpath.com/ (401 challenge)\n  - https://dealpath.stoplight.io/docs/dealpath-api\nevidence:\n- source: https://api.dealpath.com/\n  status: 401\n  detail: 'message: No authorization token found in the request header. Please obtain an auth token from Dealpath.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealpath/refs/heads/main/authentication/dealpath-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Real Estate
- PropTech
- Deal Management
- Commercial Real Estate
- Investment Management
- Real Estate Technology
- API
---
