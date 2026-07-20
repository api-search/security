---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Enverus Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Enverus secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Enverus
provider_slug: enverus
scheme_count: 3
schemes:
- description: An Enverus-issued API key is presented on every request (and on the token request) via the X-Api-Key header.
  in: header
  name: ApiKey
  parameter: X-Api-Key
  type: apiKey
- description: A client_id and client_secret are exchanged at the token endpoint (grant type client_credentials, HTTP Basic authentication of client_id:client_secret plus the X-Api-Key header) for a short-lived bearer access token.
  flow: clientCredentials
  name: ClientCredentials
  token_url: https://di-api.drillinginfo.com/v2/direct-access/tokens
  type: oauth2
- description: 'The access token returned by the token endpoint is sent as Authorization: Bearer <access_token> on all subsequent dataset queries.'
  name: BearerToken
  scheme: bearer
  type: http
slug: enverus-authentication
source_filename: enverus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://app.enverus.com/direct/#/api/explorer/v2/gettingStarted\ndocs: https://app.enverus.com/direct/#/api/explorer/v2/gettingStarted\nnote: >-\n  Derived from the documented DirectAccess API v2 authentication flow (Enverus\n  developer docs and the community directaccess client). No OpenAPI is published\n  publicly (the API explorer and specs sit behind login), so this profile is\n  authored from the documented token-exchange behavior rather than derived from\n  a spec.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: >-\n    An Enverus-issued API key is presented on every request (and on the token\n    request) via the X-Api-Key header.\n- name: ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://di-api.drillinginfo.com/v2/direct-access/tokens\n\
  \  description: >-\n    A client_id and client_secret are exchanged at the token endpoint (grant\n    type client_credentials, HTTP Basic authentication of client_id:client_secret\n    plus the X-Api-Key header) for a short-lived bearer access token.\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    The access token returned by the token endpoint is sent as\n    Authorization: Bearer <access_token> on all subsequent dataset queries.\nflow:\n- step: request-token\n  method: POST\n  url: https://di-api.drillinginfo.com/v2/direct-access/tokens\n  sends: [X-Api-Key header, Basic client_id:client_secret]\n  returns: access_token (bearer)\n- step: query\n  method: GET\n  url: https://di-api.drillinginfo.com/v2/direct-access/{dataset}\n  sends: [Authorization Bearer access_token, X-Api-Key header]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enverus/refs/heads/main/authentication/enverus-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Energy
- Oil and Gas
- Energy Data
- Analytics
- Market Intelligence
- Well Data
- SaaS
- DirectAccess
- Trading and Risk
---
