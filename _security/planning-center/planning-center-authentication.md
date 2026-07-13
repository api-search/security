---
api_key_in: []
api_specs:
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center People API
  slug: planning-center-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Services API
  slug: planning-center-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Giving API
  slug: planning-center-giving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Groups API
  slug: planning-center-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Check-Ins API
  slug: planning-center-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Calendar API
  slug: planning-center-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Registrations API
  slug: planning-center-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Publishing API
  slug: planning-center-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
- filename: planning-center-openapi.yml
  format: yaml
  label: Planning Center Webhooks API
  slug: planning-center-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/openapi/planning-center-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Planning Center Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Planning Center secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Planning Center
provider_slug: planning-center
scheme_count: 2
schemes:
- description: HTTP Basic auth using a Personal Access Token - application id as the username and secret as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/planning-center-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://api.planningcenteronline.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://api.planningcenteronline.com/oauth/token
  name: oauth2
  sources:
  - openapi/planning-center-openapi.yml
  type: oauth2
slug: planning-center-authentication
source_filename: planning-center-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/planning-center-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using a Personal Access Token - application id as the username\n    and secret as the password.\n  sources:\n  - openapi/planning-center-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.planningcenteronline.com/oauth/authorize\n    tokenUrl: https://api.planningcenteronline.com/oauth/token\n    scopes: 8\n  sources:\n  - openapi/planning-center-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/authentication/planning-center-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Church Management
- ChMS
- Faith
- Giving
- Events
- Scheduling
- People
- Nonprofit
---
