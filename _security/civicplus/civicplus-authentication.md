---
api_key_in: []
api_specs:
- filename: civicplus-seeclickfix-open311-openapi-original.yml
  format: yaml
  label: SeeClickFix API v2
  slug: seeclickfix-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civicplus/refs/heads/main/openapi/civicplus-seeclickfix-open311-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Civicplus Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CivicPlus secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CivicPlus
provider_slug: civicplus
scheme_count: 3
schemes:
- description: 'Token authentication for API access. A Personal Access Token (a Bearer token) is created under Password & Security > Personal Access Token and sent on every request as an Authorization header. Format: "Authorization: Bearer [token]".'
  header: 'Authorization: Bearer [token]'
  name: PersonalAccessToken
  scheme: bearer
  sources:
  - https://dev.seeclickfix.com/v2/overview/authentication/
  type: http
- description: OAuth2 authorization code flow (RFC 6749, implemented with Doorkeeper) for client applications used by multiple users where end-user credentials must not be shared with the client. Applications must be registered with SeeClickFix (email request) to receive an application id and callback URI before use.
  flows:
  - flow: authorizationCode
    registration: manual (email SeeClickFix developer support to register an app)
  name: OAuth2
  sources:
  - https://dev.seeclickfix.com/v2/overview/authentication/
  type: oauth2
- description: Query-parameter API key declared by the Open311 GeoReport v2 spec published in the SeeClickFix GitHub org; applies to the Open311-compatible endpoint at seeclickfix.com/open311.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/civicplus-seeclickfix-open311-openapi-original.yml
  type: apiKey
slug: civicplus-authentication
source_filename: civicplus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://dev.seeclickfix.com/v2/overview/authentication/\ndocs: https://dev.seeclickfix.com/v2/overview/authentication/\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  description: >-\n    Token authentication for API access. A Personal Access Token (a Bearer\n    token) is created under Password & Security > Personal Access Token and\n    sent on every request as an Authorization header. Format:\n    \"Authorization: Bearer [token]\".\n  header: 'Authorization: Bearer [token]'\n  sources: [https://dev.seeclickfix.com/v2/overview/authentication/]\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth2 authorization code flow (RFC 6749, implemented with Doorkeeper) for\n    client applications used by multiple users where end-user credentials must\n    not be shared with the client. Applications must\
  \ be registered with\n    SeeClickFix (email request) to receive an application id and callback URI\n    before use.\n  flows:\n  - flow: authorizationCode\n    registration: manual (email SeeClickFix developer support to register an app)\n  sources: [https://dev.seeclickfix.com/v2/overview/authentication/]\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: >-\n    Query-parameter API key declared by the Open311 GeoReport v2 spec published\n    in the SeeClickFix GitHub org; applies to the Open311-compatible endpoint at\n    seeclickfix.com/open311.\n  sources: [openapi/civicplus-seeclickfix-open311-openapi-original.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civicplus/refs/heads/main/authentication/civicplus-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Government
- GovTech
- Local Government
- 311
- Civic Engagement
- Public Records
- Service Requests
---
