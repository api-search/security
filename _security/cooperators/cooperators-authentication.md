---
api_key_in: []
api_specs:
- filename: cooperators-duuo-platform-openapi.yml
  format: yaml
  label: Duuo Platform API
  slug: duuo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cooperators/refs/heads/main/openapi/cooperators-duuo-platform-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cooperators Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: The Co-operators secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: The Co-operators
provider_slug: cooperators
scheme_count: 2
schemes:
- description: Bearer token obtained from the partner-issued OAuth 2.0 token endpoint. The token expires every 60 minutes and must be refreshed.
  name: duuoBearer
  scheme: bearer
  sources:
  - openapi/cooperators-duuo-platform-openapi.yml
  type: http
- description: OAuth 2.0 client credentials grant. POST grant_type=client_credentials to the token URL supplied by the Duuo partnerships team, with an HTTP Basic Authorization header of "Basic " + Base64("client_id" + ":" + "client_secret"). No scopes are published. The token URL is partner-issued and is not a public endpoint, so the tokenUrl below is a placeholder.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://your-partner-token-host/oauth/token
  name: duuoOAuth2
  sources:
  - openapi/cooperators-duuo-platform-openapi.yml
  type: oauth2
slug: cooperators-authentication
source_filename: cooperators-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/cooperators-duuo-platform-openapi.yml\ndocs: https://web.archive.org/web/20240127073206id_/https://developer.duuo.ca/api/collections/26639007/2s93sXcubU\ndocs_note: >-\n  Duuo's own published Authorization documentation, retrieved from the Internet Archive capture of\n  its developer-portal Postman collection. The live portal (https://developer.duuo.ca/) returns 404\n  as of 2026-07-25. Co-operators' own advisor/broker surface is sign-in walls only and documents no\n  API authentication at all.\ntoken_flow:\n  protocol: OAuth 2.0\n  grant_type: client_credentials\n  token_endpoint: partner-issued (no public token URL is published)\n  client_authentication: >-\n    HTTP Basic — 'Authorization: Basic ' + Base64Encoded(\"client_id\" + \":\" + \"client_secret\")\n  request_body: '{\"grant_type\":\"client_credentials\"}'\n  response_fields: [access_token, expires_in, token_type]\n  token_type: Bearer\n  expires_in: 3600\n\
  \  refresh: >-\n    Duuo states the token expires every 60 minutes and should therefore be refreshed. There is no\n    refresh_token in a client_credentials flow — re-run the token call.\n  call_header: 'Authorization: Bearer {access_token}'\ncredential_issuance:\n  self_serve: false\n  process: >-\n    Discovery call with the Duuo partnerships team, signed partnership agreement, assigned Partner\n    Account Manager, then issued API access credentials and a partner-specific host. A compliance\n    review of the implementation is required before go-live.\n  signup: https://duuo.ca/new-partners/\nauthorization_model:\n  scopes: none published\n  enforcement: >-\n    Per-partner entitlement enforced server-side. An unentitled call returns 403 \"Access Denied -\n    Requires Access Mgmt\" with responseDetails \"Access denied.\"\n  mtls: false\n  ip_allowlist: not documented\ndiscovery:\n  openid_configuration: 404 on cooperators.ca and duuo.ca (probed 2026-07-25)\n  oauth_authorization_server:\
  \ 404 on cooperators.ca (probed 2026-07-25)\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: duuoBearer\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from the partner-issued OAuth 2.0 token endpoint. The token\n    expires every 60 minutes and must be refreshed.\n  sources:\n  - openapi/cooperators-duuo-platform-openapi.yml\n- name: duuoOAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-partner-token-host/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials grant. POST grant_type=client_credentials to the\n    token URL supplied by the Duuo partnerships team, with an HTTP Basic Authorization header\n    of \"Basic \" + Base64(\"client_id\" + \":\" + \"client_secret\"). No scopes are published. The\n    token URL is partner-issued and is not a public endpoint, so the tokenUrl below is a placeholder.\n  sources:\n  - openapi/cooperators-duuo-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooperators/refs/heads/main/authentication/cooperators-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Insurance
- Canada
- Property and Casualty
- Life Insurance
- Group Benefits
- Embedded Insurance
- Cooperative
- Wealth Management
- Partner API
---
