---
anonymous_access: false
api_key_in: []
api_specs:
- filename: codebeamer-openapi-generated.yml
  format: yaml
  label: Codebeamer REST API (Swagger v3)
  slug: codebeamer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebeamer/openapi/_ae-authored/codebeamer-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Codebeamer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codebeamer declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Codebeamer
provider_slug: codebeamer
scheme_count: 4
schemes:
- description: This option uses the HTTP basic authentication method, in which the username and password are provided as an encoded authorization header.
  name: basic
  scheme: basic
  type: http
- bearerFormat: OpenID Connect access token
  description: In the bearer authentication the OpenID is configured as an authentication layer in Codebeamer. It is the user's responsibility to acquire the access token from the OpenID provider.
  name: bearer
  scheme: bearer
  type: http
- authorizationUrl: cb/api/oauth2/authorize.spr
  description: Web-based authentication for Codebeamer and third-party applications (authorization code grant; token response carries access_token, token_type, expires_in, refresh_token). Paths are relative to each customer instance.
  docs: https://support.ptc.com/help/codebeamer/r3.2/en/codebeamer/developers_guide/swagger/dg_swagger_web_based_authentication.html
  flow: authorizationCode
  name: oauth2-authorization-code
  scopes:
  - API
  tokenUrl: cb/api/oauth2/token
  type: oauth2
- description: This is for internal use only. As our internal processes rely on our API, this method is used to authenticate between our components.
  internal_only: true
  name: api-key
  type: apiKey
slug: codebeamer-authentication
source_filename: codebeamer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://support.ptc.com/help/codebeamer/r3.2/en/codebeamer/developers_guide/swagger/11375898.html\ndocs: https://support.ptc.com/help/codebeamer/r3.2/en/codebeamer/developers_guide/swagger/11375898.html\nsummary: Every Codebeamer API call must be authenticated as a registered user; the user must belong to a group with the \"Rest / Remote API - Access\" permission and have at least read permission on the requested resource.\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: This option uses the HTTP basic authentication method, in which the username and password are provided as an encoded authorization header.\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: OpenID Connect access token\n  description: In the bearer authentication the OpenID is configured as an authentication layer in Codebeamer. It is the user's responsibility to acquire the access token from the OpenID provider.\n- name:\
  \ oauth2-authorization-code\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: cb/api/oauth2/authorize.spr\n  tokenUrl: cb/api/oauth2/token\n  scopes: [API]\n  docs: https://support.ptc.com/help/codebeamer/r3.2/en/codebeamer/developers_guide/swagger/dg_swagger_web_based_authentication.html\n  description: Web-based authentication for Codebeamer and third-party applications (authorization code grant; token response carries access_token, token_type, expires_in, refresh_token). Paths are relative to each customer instance.\n- name: api-key\n  type: apiKey\n  internal_only: true\n  description: This is for internal use only. As our internal processes rely on our API, this method is used to authenticate between our components.\nnote: Codebeamer is deployed per customer; there is no shared public API host, so endpoints are relative to the instance's site URL.\n"
source_yaml_url: https://artifacts.apis.io/codebeamer/authentication/codebeamer-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Application Lifecycle Management
- Requirements Management
- Software Engineering
- Test Management
- Risk Management
- DevOps
- PTC
---
