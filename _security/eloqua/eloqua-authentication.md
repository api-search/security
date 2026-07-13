---
api_key_in: []
api_specs:
- filename: eloqua-rest-openapi.yml
  format: yaml
  label: Eloqua REST API
  slug: eloqua-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/openapi/eloqua-rest-openapi.yml
- filename: eloqua-bulk-openapi.yml
  format: yaml
  label: Eloqua Bulk API
  slug: eloqua-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/openapi/eloqua-bulk-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Eloqua Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Oracle Eloqua secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Oracle Eloqua
provider_slug: eloqua
scheme_count: 2
schemes:
- description: HTTP Basic authentication using company\username and password in the format CompanyName\Username.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/eloqua-bulk-openapi.yml
  - openapi/eloqua-rest-openapi.yml
  type: http
- description: OAuth 2.0 authorization code flow
  flows:
  - authorizationUrl: https://login.eloqua.com/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.eloqua.com/auth/oauth2/token
  name: oAuth2
  sources:
  - openapi/eloqua-bulk-openapi.yml
  - openapi/eloqua-rest-openapi.yml
  type: oauth2
slug: eloqua-authentication
source_filename: eloqua-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eloqua-bulk-openapi.yml, openapi/eloqua-rest-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using company\\username and password in the format CompanyName\\Username.\n  sources:\n  - openapi/eloqua-bulk-openapi.yml\n  - openapi/eloqua-rest-openapi.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.eloqua.com/auth/oauth2/authorize\n    tokenUrl: https://login.eloqua.com/auth/oauth2/token\n    scopes: 1\n  description: OAuth 2.0 authorization code flow\n  sources:\n  - openapi/eloqua-bulk-openapi.yml\n  - openapi/eloqua-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/authentication/eloqua-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- CRM
- Email Marketing
- Lead Management
- Marketing Automation
---
