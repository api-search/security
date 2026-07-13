---
api_key_in: []
api_specs:
- filename: xmatters-openapi.yml
  format: yaml
  label: xMatters REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/openapi/xmatters-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Xmatters Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: xMatters secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: xMatters
provider_slug: xmatters
scheme_count: 2
schemes:
- description: HTTP Basic authentication using a username and password or API key.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/xmatters-openapi.yml
  type: http
- flows:
  - flow: password
    scopes: 0
    tokenUrl: https://{company}.{deployment}.xmatters.com/api/xm/1/oauth2/token
  name: OAuth2
  sources:
  - openapi/xmatters-openapi.yml
  type: oauth2
slug: xmatters-authentication
source_filename: xmatters-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xmatters-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using a username and password or API key.\n  sources:\n  - openapi/xmatters-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://{company}.{deployment}.xmatters.com/api/xm/1/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/xmatters-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xmatters/refs/heads/main/authentication/xmatters-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Incident Management
- On-Call
- Alerting
- Service Reliability
- DevOps
- Communication
- Workflow Automation
---
