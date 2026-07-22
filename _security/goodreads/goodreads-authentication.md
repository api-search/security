---
api_key_in:
- query
auth_types:
- openIdConnect
- oauth1
description: ''
kind: authentication
layout: security
method: searched
name: Goodreads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goodreads secures its APIs with openIdConnect and oauth1 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Goodreads
provider_slug: goodreads
scheme_count: 3
schemes:
- authorization_endpoint: https://www.goodreads.com/open_id/auth_token
  description: OpenID Connect discovery for signing in with a Goodreads account.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://www.goodreads.com
  jwks_uri: https://www.goodreads.com/open_id/keys
  name: OpenIDConnect
  openIdConnectUrl: https://www.goodreads.com/.well-known/openid-configuration
  response_types_supported:
  - code
  - token
  sources:
  - well-known/goodreads-openid-configuration.json
  type: openIdConnect
- description: The legacy public Goodreads REST/XML API authenticated public reads with a developer `key` query parameter and used OAuth 1.0a for user-scoped calls. Goodreads stopped issuing new developer keys on 2020-12-08 (see lifecycle); kept here for historical accuracy, not as an available scheme.
  in: query
  name: LegacyDeveloperKey
  parameter: key
  sources:
  - https://www.goodreads.com/api
  status: retired
  type: apiKey
- description: OAuth 1.0a user authorization used by the retired public developer API for member-scoped operations (shelves, reviews). No longer accepting new apps.
  name: LegacyOAuth1
  sources:
  - https://www.goodreads.com/api
  status: retired
  type: oauth1
slug: goodreads-authentication
source_filename: goodreads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.goodreads.com/.well-known/openid-configuration\ndocs: https://www.goodreads.com/api\nsummary:\n  types: [openIdConnect, oauth1]\n  api_key_in: [query]\n  oauth2_flows: []\n  notes: >-\n    No OpenAPI is published for Goodreads, so this profile is searched from\n    the live OpenID Connect discovery document and the (now-retired) public\n    developer API documentation rather than derived from a spec.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.goodreads.com/.well-known/openid-configuration\n  issuer: https://www.goodreads.com\n  authorization_endpoint: https://www.goodreads.com/open_id/auth_token\n  jwks_uri: https://www.goodreads.com/open_id/keys\n  response_types_supported: [code, token]\n  id_token_signing_alg_values_supported: [RS256]\n  sources: [well-known/goodreads-openid-configuration.json]\n  description: >-\n    OpenID Connect discovery for signing in with a\
  \ Goodreads account.\n- name: LegacyDeveloperKey\n  type: apiKey\n  in: query\n  parameter: key\n  status: retired\n  sources: [https://www.goodreads.com/api]\n  description: >-\n    The legacy public Goodreads REST/XML API authenticated public reads with\n    a developer `key` query parameter and used OAuth 1.0a for user-scoped\n    calls. Goodreads stopped issuing new developer keys on 2020-12-08 (see\n    lifecycle); kept here for historical accuracy, not as an available scheme.\n- name: LegacyOAuth1\n  type: oauth1\n  status: retired\n  sources: [https://www.goodreads.com/api]\n  description: >-\n    OAuth 1.0a user authorization used by the retired public developer API for\n    member-scoped operations (shelves, reviews). No longer accepting new apps.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodreads/refs/heads/main/authentication/goodreads-authentication.yml
summary_line: openIdConnect/oauth1 · 3 schemes
tags:
- Company
- Consumer
- Books
- Reading
- Social Network
- Recommendations
- Reviews
- Amazon
---
