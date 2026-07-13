---
api_key_in:
- cookie
api_specs:
- filename: drupal-rest-api-openapi.yml
  format: yaml
  label: Drupal REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-rest-api-openapi.yml
- filename: drupal-jsonapi-openapi.yml
  format: yaml
  label: Drupal JSON:API
  slug: jsonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/openapi/drupal-jsonapi-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Drupal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: drupal secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: drupal
provider_slug: drupal
scheme_count: 3
schemes:
- description: HTTP Basic Authentication using Drupal username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/drupal-jsonapi-openapi.yml
  - openapi/drupal-rest-api-openapi.yml
  type: http
- description: Cookie-based session authentication obtained via Drupal login.
  in: cookie
  name: cookieAuth
  parameter: SESS
  sources:
  - openapi/drupal-jsonapi-openapi.yml
  - openapi/drupal-rest-api-openapi.yml
  type: apiKey
- description: OAuth 2.0 via the Simple OAuth module.
  flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://example.com/oauth/token
  name: oAuth2
  sources:
  - openapi/drupal-jsonapi-openapi.yml
  - openapi/drupal-rest-api-openapi.yml
  type: oauth2
slug: drupal-authentication
source_filename: drupal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drupal-jsonapi-openapi.yml, openapi/drupal-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Drupal username and password.\n  sources:\n  - openapi/drupal-jsonapi-openapi.yml\n  - openapi/drupal-rest-api-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: SESS\n  description: Cookie-based session authentication obtained via Drupal login.\n  sources:\n  - openapi/drupal-jsonapi-openapi.yml\n  - openapi/drupal-rest-api-openapi.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 via the Simple OAuth module.\n  sources:\n  - openapi/drupal-jsonapi-openapi.yml\n\
  \  - openapi/drupal-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/authentication/drupal-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags: []
---
