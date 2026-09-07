---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Sempra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sempra secures its APIs with http across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sempra
provider_slug: sempra
scheme_count: 0
schemes: []
slug: sempra-authentication
source_filename: sempra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  Live unauthenticated HTTP probes of https://api.sempra.com on 2026-09-04. Sempra\n  publishes no authentication documentation on any public surface, so every statement\n  below is read directly off the gateway's own responses. Host ownership is established\n  from the DigiCert EV certificate on api.sempra.com — subject O=Sempra Energy,\n  L=San Diego, ST=California, C=US, serialNumber 2062548, issuer DigiCert EV RSA CA G2.\napi: Sempra Developer Portal APIs\nbase_url: https://api.sempra.com/v1\ngateway: Google Apigee\ndocs: null\ndocs_note: >-\n  There is no public authentication page. https://developer.sempra.com requires\n  registration; its anonymous catalog endpoint\n  /portals/api/sites/sempra-prod/liveportal/apis returns HTTP 200 with apiDocs [] and\n  apiProducts [], and its header menu is exactly \"APIs\" and \"Log In\".\nnote: >-\n  api.sempra.com is an Apigee runtime. A request to \"/\" returns the Apigee\n  messaging.adaptors.http.flow.ApplicationNotFound\
  \ fault (HTTP 404), meaning no proxy is\n  routed there. A proxy IS routed at basepath /v1: every path under /v1 — including\n  /v1, /v1/graphql, /v1/token and /v1/openapi.json — returns HTTP 401 with an Apigee\n  OAuthV2 fault, while /v2/graphql, /oauth/token, /openapi.json, /swagger.json,\n  /api-docs and /docs return the not-routed 404. That contrast is the evidence that /v1\n  is a real, live, OAuth-protected API basepath. No token issuance endpoint is\n  discoverable anonymously and no scope, grant type or client registration flow is\n  published — credentials are obtained by registering on https://developer.sempra.com.\nsummary:\n  types: [http]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Scheme list is what the gateway demonstrates, not what a spec declares — Sempra\n    publishes no OpenAPI, so nothing here is derived from a contract.\nsecurity_schemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: OAuth 2.0 access token (Apigee OAuthV2)\n  in:\
  \ header\n  header: Authorization\n  method: probed\n  evidence:\n    request: GET https://api.sempra.com/v1/graphql\n    status: 401\n    www_authenticate: >-\n      Bearer realm=\"null\",error=\"invalid_token\",error_description=\"oauth.v2.InvalidAccessToken:\n      Invalid access token\"\n    body: '{\"fault\":{\"faultstring\":\"Invalid access token\",\"detail\":{\"errorcode\":\"oauth.v2.InvalidAccessToken\"}}}'\n  note: >-\n    RFC 6750 bearer challenge emitted by an Apigee OAuthV2 VerifyAccessToken policy.\noauth2:\n  detected: true\n  detection: Apigee OAuthV2 VerifyAccessToken policy (oauth.v2.InvalidAccessToken fault)\n  token_endpoint: null\n  authorization_endpoint: null\n  grant_types: []\n  scopes: []\n  note: >-\n    No token, authorization or discovery endpoint is reachable anonymously.\n    /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource\n    both return the Apigee not-routed 404 on api.sempra.com; /oauth/token is not routed;\n    /v1/token\
  \ is routed but rejects at the OAuth policy before any grant is processed.\n    Grant types and scopes are undocumented publicly, so scopes/ is deliberately not\n    written — there is nothing real to put in it.\ntransport:\n  tls: true\n  tls_version: TLSv1.2\n  hsts: max-age=31536000 (observed on the /v1 proxy response)\n  content_security_policy: \"script-src 'self'; child-src 'self'; form-action 'self'\"\n  cors:\n    access_control_allow_origin: '*'\n    access_control_allow_headers: '*'\n    access_control_allow_methods: GET, PUT, POST, DELETE, OPTIONS, PATCH\n    access_control_max_age: 3628800\n    note: >-\n      A permissive wildcard CORS policy advertising six HTTP methods, which indicates a\n      browser-callable read/write surface behind the token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sempra/refs/heads/main/authentication/sempra-authentication.yml
summary_line: http · 0 schemes
tags:
- Energy
- Utilities
- Natural Gas
- Electricity
- Energy Infrastructure
- LNG
- Apigee
- Fortune 500
---
