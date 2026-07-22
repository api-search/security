---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: On24 Authentication
name_suffix: Authentication
oauth_flows: []
overview: On24 secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: On24
provider_slug: on24
scheme_count: 2
schemes:
- description: Per-client API token key issued in the ON24 platform (Account > Integrations / API access). Sent as the `accessTokenKey` request header.
  in: header
  key_name: accessTokenKey
  name: accessTokenKey
  type: apiKey
- description: Secret paired with accessTokenKey. Sent as the `accessTokenSecret` request header alongside accessTokenKey.
  in: header
  key_name: accessTokenSecret
  name: accessTokenSecret
  type: apiKey
slug: on24-authentication
source_filename: on24-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://apidoc.on24.com/ (ON24 API documentation portal) and the ON24 client\n  contract confirmed in the community node-on24 client source\n  (github.com/the-automaton/node-on24, src/client-base.ts). ON24 publishes no\n  first-party OpenAPI, so the auth model is captured from the docs + a live\n  client rather than derived from a spec.\ndocs: https://apidoc.on24.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    ON24 authenticates every request with a numeric client id embedded in the\n    URL path plus a token key/secret pair sent as HTTP request headers. There is\n    no OAuth 2.0 / OIDC surface documented.\nschemes:\n- name: accessTokenKey\n  type: apiKey\n  in: header\n  key_name: accessTokenKey\n  description: >-\n    Per-client API token key issued in the ON24 platform (Account > Integrations\n    / API access). Sent as the `accessTokenKey` request header.\n- name: accessTokenSecret\n\
  \  type: apiKey\n  in: header\n  key_name: accessTokenSecret\n  description: >-\n    Secret paired with accessTokenKey. Sent as the `accessTokenSecret` request\n    header alongside accessTokenKey.\nclient_scope:\n  in: path\n  parameter: clientId\n  description: >-\n    Numeric ON24 client (account) id scoping every call; forms part of the base\n    path https://api.on24.com/v2/client/{clientId}/...\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/on24/refs/heads/main/authentication/on24-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Webinars
- Virtual Events
- Digital Engagement
- Marketing
- Analytics
- Event Management
- Martech
---
