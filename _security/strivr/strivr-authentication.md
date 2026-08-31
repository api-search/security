---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Strivr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Strivr declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Strivr
provider_slug: strivr
scheme_count: 2
schemes:
- applies_to:
  - https://portal.strivr.com/
  - Strivr SDK Unity Editor window (Strivr > Project Settings > Log in)
  description: 'Access to the Strivr Portal is single sign-on, brokered by Auth0. The documented entry point is "Log in with Google" at portal.strivr.com. Self-service signup does not exist: the docs instruct you to contact Strivr with a list of users at your company, after which Strivr configures SSO and issues credentials, and the user verifies identity via an email from Auth0.'
  evidence: https://developer.strivr.com/docs/sdk/latest/unity/access-strivr-portal.html
  flow: browser redirect / SSO
  name: portal_sso
  provider: Auth0
  self_service: false
  type: openIdConnect
- applies_to:
  - https://api.strivr.com
  description: 'The Strivr API host answers every unauthenticated request - including / , /openapi.json and every /.well-known/ path - with HTTP 401 and the response header WWW-Authenticate: Bearer, with a zero-length body. This establishes a bearer-token model on the wire. Strivr does not publish how a token is obtained, its lifetime, its format, or any scope vocabulary.'
  evidence:
    http_status: 401
    response_header: 'WWW-Authenticate: Bearer'
    server: Apache/2.4.58 (Ubuntu)
    url: https://api.strivr.com/
  header: Authorization
  in: header
  method: probed
  name: api_bearer
  scheme: bearer
  type: http
slug: strivr-authentication
source_filename: strivr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://developer.strivr.com/docs/sdk/latest/unity/getting-started.html, https://developer.strivr.com/docs/sdk/latest/unity/access-strivr-portal.html,\n  https://developer.strivr.com/docs/sdk/latest/unity/linking-unity-to-strivr.html, live probe of https://api.strivr.com/\ndocs: https://developer.strivr.com/docs/sdk/latest/unity/getting-started.html\nnote: Derived from the published SDK documentation and one live probe, NOT from an OpenAPI - Strivr publishes\n  no securitySchemes because it publishes no machine-readable contract. Every fact below is either stated\n  in Strivr's own docs or observed on the wire.\nschemes:\n- name: portal_sso\n  type: openIdConnect\n  provider: Auth0\n  flow: browser redirect / SSO\n  applies_to:\n  - https://portal.strivr.com/\n  - Strivr SDK Unity Editor window (Strivr > Project Settings > Log in)\n  description: 'Access to the Strivr Portal is single sign-on, brokered by Auth0. The documented\
  \ entry\n    point is \"Log in with Google\" at portal.strivr.com. Self-service signup does not exist: the docs instruct\n    you to contact Strivr with a list of users at your company, after which Strivr configures SSO and\n    issues credentials, and the user verifies identity via an email from Auth0.'\n  self_service: false\n  evidence: https://developer.strivr.com/docs/sdk/latest/unity/access-strivr-portal.html\n- name: api_bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  applies_to:\n  - https://api.strivr.com\n  description: 'The Strivr API host answers every unauthenticated request - including / , /openapi.json\n    and every /.well-known/ path - with HTTP 401 and the response header WWW-Authenticate: Bearer, with\n    a zero-length body. This establishes a bearer-token model on the wire. Strivr does not publish how\n    a token is obtained, its lifetime, its format, or any scope vocabulary.'\n  method: probed\n  evidence:\n    url: https://api.strivr.com/\n\
  \    http_status: 401\n    response_header: 'WWW-Authenticate: Bearer'\n    server: Apache/2.4.58 (Ubuntu)\nunity_editor_flow: In Unity, Strivr > Project Settings > Log in opens a web page to complete the login\n  flow; after login the developer selects which Strivr project the Unity project is linked to. The selection\n  persists across editor sessions.\noauth_scopes_published: false\napi_keys_published: false\nmtls: false\ngaps:\n- No token issuance or refresh documentation\n- No scope vocabulary\n- No public OAuth metadata document (all /.well-known/ paths on api.strivr.com are themselves 401-gated)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strivr/refs/heads/main/authentication/strivr-authentication.yml
summary_line: 2 schemes
tags:
- Immersive Learning
- Virtual Reality
- Workforce Training
- Frontline Operations
- Artificial Intelligence
- Analytics
- Unity SDK
- Smart Glasses
- Enterprise
- Learning and Development
---
