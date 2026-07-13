---
api_key_in: []
api_specs:
- filename: v2.json
  format: json
  label: Red Hat Satellite REST API
  slug: red-hat-satellite-rest-api
  spec_type: OpenAPI
  url: https://satellite.example.com/apidoc/v2.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Red Hat Satellite Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Red Hat Satellite secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
scheme_count: 2
schemes:
- description: HTTP Basic authentication using Satellite username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/red-hat-satellite-api.yml
  type: http
- description: OAuth 2.0 Personal Access Token authentication for Satellite users.
  flows:
  - authorizationUrl: https://satellite.example.com/users/extlogin
    flow: implicit
    scopes: 0
  name: oAuth2
  sources:
  - openapi/red-hat-satellite-api.yml
  type: oauth2
slug: red-hat-satellite-authentication
source_filename: red-hat-satellite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/red-hat-satellite-api.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using Satellite username and password.\n  sources:\n  - openapi/red-hat-satellite-api.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://satellite.example.com/users/extlogin\n    scopes: 0\n  description: OAuth 2.0 Personal Access Token authentication for Satellite users.\n  sources:\n  - openapi/red-hat-satellite-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/authentication/red-hat-satellite-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
---
