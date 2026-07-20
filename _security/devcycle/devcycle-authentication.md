---
api_key_in:
- header
api_specs:
- filename: devcycle-management-openapi.json
  format: json
  label: DevCycle Management API
  slug: devcycle-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/openapi/devcycle-management-openapi.json
- filename: devcycle-bucketing-openapi.yaml
  format: yaml
  label: DevCycle Bucketing API
  slug: devcycle-bucketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/openapi/devcycle-bucketing-openapi.yaml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Devcycle Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: DevCycle secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: DevCycle
provider_slug: devcycle
scheme_count: 2
schemes:
- api: DevCycle Management API
  credentials: Client ID + Secret from the DevCycle dashboard (Settings > API Authentication)
  enterprise_grant:
    grant_type: refresh_token
    note: for organizations with strict role-based access control enabled
  flows:
  - audience: https://api.devcycle.com/
    flow: clientCredentials
    grant_type: client_credentials
    scopes: {}
    tokenUrl: https://auth.devcycle.com/oauth/token
  name: managementOAuth2
  source: https://docs.devcycle.com/management-api/
  type: oauth2
- api: DevCycle Bucketing API
  description: DevCycle server SDK key, sent as a bearer token
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/devcycle-bucketing-openapi.yaml
  type: apiKey
slug: devcycle-authentication
source_filename: devcycle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.devcycle.com/management-api/\ndocs: https://docs.devcycle.com/management-api/\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nnotes: >-\n  DevCycle exposes two API surfaces with distinct auth models. The Management API\n  (api.devcycle.com) uses OAuth2 client_credentials against the Auth0 tenant\n  (auth.devcycle.com) with an audience of https://api.devcycle.com/; an enterprise\n  refresh_token grant is offered for organizations with strict RBAC. The Bucketing\n  API (bucketing-api.devcycle.com) authenticates with a DevCycle server SDK key\n  passed as a bearer token in the Authorization header. No OAuth scopes are\n  documented - access is audience-based, not scope-based.\nschemes:\n- name: managementOAuth2\n  type: oauth2\n  api: DevCycle Management API\n  source: https://docs.devcycle.com/management-api/\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://auth.devcycle.com/oauth/token\n    audience: https://api.devcycle.com/\n    grant_type: client_credentials\n    scopes: {}\n  enterprise_grant:\n    grant_type: refresh_token\n    note: for organizations with strict role-based access control enabled\n  credentials: Client ID + Secret from the DevCycle dashboard (Settings > API Authentication)\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: DevCycle server SDK key, sent as a bearer token\n  api: DevCycle Bucketing API\n  sources:\n  - openapi/devcycle-bucketing-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/authentication/devcycle-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Enterprise Saas
- Feature Flags
- Feature Management
- Feature Flags as a Service
- Experimentation
- OpenFeature
- Developer Tools
- DevOps
---
