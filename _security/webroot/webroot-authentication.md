---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Webroot Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Webroot secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Webroot
provider_slug: webroot
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth2 resource-owner password-credentials grant using Unity API user credentials (client id/secret + username/password), returning an access token used as an Authorization: Bearer token on /service/api calls.'
  flow: password
  name: UnityOAuth2
  sources:
  - probe:https://unityapi.webrootcloudav.com/auth/token
  tokenUrl: https://unityapi.webrootcloudav.com/auth/token
  type: oauth2
slug: webroot-authentication
source_filename: webroot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://unityapi.webrootcloudav.com/docs\ndocs: https://unityapi.webrootcloudav.com/docs\nnotes: >-\n  The Webroot Unity API authenticates with OAuth2. A single token is obtained\n  from the token endpoint and then presented as a bearer token on subsequent\n  REST calls. Verified live: the token endpoint https://unityapi.webrootcloudav.com/auth/token\n  returns HTTP 400 (application/json) to an unauthenticated request, and\n  protected resources under /service/api (e.g. /service/api/console/gsm) return\n  HTTP 401 (application/json) without a token. Access is scoped to a customer's\n  Unity API user credentials; there is no public self-serve signup.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\n  bearer: true\nschemes:\n- name: UnityOAuth2\n  type: oauth2\n  flow: password\n  tokenUrl: https://unityapi.webrootcloudav.com/auth/token\n  bearerFormat: JWT\n  description: >-\n    OAuth2 resource-owner password-credentials\
  \ grant using Unity API user\n    credentials (client id/secret + username/password), returning an access\n    token used as an Authorization: Bearer token on /service/api calls.\n  sources:\n  - probe:https://unityapi.webrootcloudav.com/auth/token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webroot/refs/heads/main/authentication/webroot-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cybersecurity
- Endpoint Protection
- Threat Intelligence
- Security
- Antivirus
- DNS Protection
- OpenText
---
