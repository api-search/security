---
api_key_in:
- query
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Constructor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Constructor secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Constructor
provider_slug: constructor
scheme_count: 3
schemes:
- description: Public index identifier used on autocomplete/search/browse/tracking requests.
  in: query
  name: apiKey
  parameter: key
  scope: public
  type: apiKey
- description: Private API token supplied as the Basic Auth username with an empty password, on privileged (catalog/config) endpoints.
  name: apiTokenBasic
  scheme: basic
  scope: private
  type: http
- description: 'Private API token supplied as Authorization: Bearer <token>. Bearer tokens support scoped permissions (r / w / rw) that may be limited to specific API keys.'
  name: apiTokenBearer
  permission_scopes:
  - code: r
    meaning: read
  - code: w
    meaning: write
  - code: rw
    meaning: read-write
  scheme: bearer
  scope: private
  type: http
slug: constructor-authentication
source_filename: constructor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.constructor.com/reference/main-authentication\ndocs: https://docs.constructor.com/reference/main-authentication\nhost: https://ac.cnstrc.com\nsummary:\n  types: [apiKey, http]\n  api_key_in: [query]\n  http_schemes: [basic, bearer]\n  oauth2_flows: []\n  notes: >-\n    Two credentials. A public API KEY identifies the index and is passed as the\n    `key` query parameter on read/tracking calls. A private API TOKEN\n    authenticates privileged calls and is passed either as the Basic Auth\n    username (no password) or as an Authorization: Bearer token. Newer Bearer\n    tokens carry explicit permission scopes (read `r`, write `w`, or read-write\n    `rw`) that can be restricted to specific API keys. This is token-based auth,\n    not OAuth 2.0.\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: query\n    parameter: key\n    description: Public index identifier used on autocomplete/search/browse/tracking requests.\n\
  \    scope: public\n  - name: apiTokenBasic\n    type: http\n    scheme: basic\n    description: >-\n      Private API token supplied as the Basic Auth username with an empty\n      password, on privileged (catalog/config) endpoints.\n    scope: private\n  - name: apiTokenBearer\n    type: http\n    scheme: bearer\n    description: >-\n      Private API token supplied as Authorization: Bearer <token>. Bearer tokens\n      support scoped permissions (r / w / rw) that may be limited to specific API keys.\n    scope: private\n    permission_scopes:\n      - {code: r, meaning: read}\n      - {code: w, meaning: write}\n      - {code: rw, meaning: read-write}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constructor/refs/heads/main/authentication/constructor-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Ecommerce
- Search
- Product Discovery
- Recommendations
- Personalization
- Retail
- AI
---
