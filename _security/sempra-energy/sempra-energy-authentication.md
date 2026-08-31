---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sempra Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sempra Energy declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Sempra Energy
provider_slug: sempra-energy
scheme_count: 0
schemes: []
slug: sempra-energy-authentication
source_filename: sempra-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: >-\n  Live unauthenticated HTTP probes of https://api.sempra.com on 2026-08-28. Sempra Energy\n  publishes no authentication documentation on any public surface, so every statement here\n  is read directly off the gateway's own responses. Host ownership is established from the\n  DigiCert EV certificate on api.sempra.com, subject O=Sempra Energy, L=San Diego,\n  ST=California, C=US.\napi: Sempra Developer Portal APIs\nbase_url: https://api.sempra.com/v1\ngateway: Google Apigee\nnote: >-\n  api.sempra.com is an Apigee runtime. Requests to \"/\" return the Apigee\n  messaging.adaptors.http.flow.ApplicationNotFound fault (HTTP 404), which means no proxy\n  is routed there. A proxy IS routed at basepath /v1: every path under /v1 (including\n  /v1/graphql, /v1/token and /v1/graphql/health) returns HTTP 401 with an Apigee OAuthV2\n  fault, while /v2/graphql and /oauth/token return the 404 not-routed fault. That contrast\n  is the evidence\
  \ that /v1 is a real, live, OAuth-protected API basepath. No token issuance\n  endpoint is discoverable anonymously and no scope, grant type or registration flow is\n  published — credentials are obtained by registering on\n  https://developer.sempra.com, whose anonymous API catalog is empty.\nsecurity_schemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: OAuth 2.0 access token (Apigee OAuthV2)\n  in: header\n  header: Authorization\n  method: probed\n  evidence:\n    request: GET https://api.sempra.com/v1/graphql\n    status: 401\n    www_authenticate: >-\n      Bearer realm=\"null\",error=\"invalid_token\",error_description=\"oauth.v2.InvalidAccessToken:\n      Invalid access token\"\n    body: '{\"fault\":{\"faultstring\":\"Invalid access token\",\"detail\":{\"errorcode\":\"oauth.v2.InvalidAccessToken\"}}}'\n  note: >-\n    RFC 6750 bearer challenge. Presenting a syntactically valid but unknown bearer token\n    changes the fault to keymanagement.service.invalid_access_token,\
  \ confirming the token is\n    validated against Apigee key management rather than merely parsed.\noauth2:\n  detected: true\n  detection: Apigee OAuthV2 VerifyAccessToken policy (oauth.v2.InvalidAccessToken fault)\n  token_endpoint: null\n  authorization_endpoint: null\n  grant_types: []\n  scopes: []\n  note: >-\n    No token, authorization or discovery endpoint is reachable anonymously.\n    /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource both\n    return the Apigee 404 not-routed fault on api.sempra.com. /oauth/token is not routed.\n    Grant types and scopes are undocumented publicly.\ntransport:\n  tls: true\n  hsts: 'max-age=31536000 (on the /v1 proxy response)'\n  cors:\n    access_control_allow_origin: '*'\n    access_control_allow_headers: '*'\n    access_control_allow_methods: GET, PUT, POST, DELETE, OPTIONS, PATCH\n    access_control_max_age: 3628800\n    note: >-\n      The gateway advertises a permissive wildcard CORS policy and six HTTP\
  \ methods,\n      which indicates a browser-callable read/write surface behind the token.\n  content_security_policy: \"script-src 'self'; child-src 'self'; form-action 'self'\"\ndocs: null\ndocs_note: >-\n  There is no public authentication page. https://developer.sempra.com requires\n  registration and its anonymous catalog endpoint returns apiDocs [] and apiProducts [].\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sempra-energy/refs/heads/main/authentication/sempra-energy-authentication.yml
summary_line: 0 schemes
tags:
- Fortune 500
- Energy
- Utilities
- Natural Gas
- Electricity
- Energy Infrastructure
- LNG
- Apigee
---
