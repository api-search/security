---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Runscope Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Runscope secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Runscope
provider_slug: runscope
scheme_count: 2
schemes:
- description: Authorization header bearer token. Accepts an OAuth2 access token or a Personal Access Token.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://help.blazemeter.com/apidocs/api-monitoring/index.htm
  type: http
- description: OAuth2 authorization-code flow for applications acting on behalf of a Runscope/BlazeMeter user.
  flows:
  - authorizationUrl: https://www.runscope.com/signin/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.runscope.com/signin/oauth/access_token
  name: oauth2
  sources:
  - https://help.blazemeter.com/apidocs/api-monitoring/index.htm
  type: oauth2
slug: runscope-authentication
source_filename: runscope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.blazemeter.com/apidocs/api-monitoring/index.htm\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nnotes: >-\n  The Runscope (now BlazeMeter API Monitoring) REST API authenticates requests\n  with a bearer token supplied in the Authorization header. Tokens are obtained\n  either through the OAuth2 authorization-code flow for third-party\n  applications, or as a Personal Access Token generated from the account's\n  Applications settings for personal/first-party use. Derived from the\n  published API reference docs; no OpenAPI is available in this repo to derive\n  a mechanical profile from.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Authorization header bearer token. Accepts an OAuth2 access token or a\n    Personal Access Token.\n  sources:\n  - https://help.blazemeter.com/apidocs/api-monitoring/index.htm\n- name: oauth2\n\
  \  type: oauth2\n  description: >-\n    OAuth2 authorization-code flow for applications acting on behalf of a\n    Runscope/BlazeMeter user.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.runscope.com/signin/oauth/authorize\n    tokenUrl: https://www.runscope.com/signin/oauth/access_token\n  sources:\n  - https://help.blazemeter.com/apidocs/api-monitoring/index.htm\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runscope/refs/heads/main/authentication/runscope-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- API Monitoring
- API Testing
- Observability
- Synthetic Monitoring
- Developer Tools
- Quality Assurance
---
