---
api_key_in: []
api_specs:
- filename: greenhouse-harvest-openapi.yml
  format: yaml
  label: Greenhouse Harvest API
  slug: harvest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-harvest-openapi.yml
- filename: greenhouse-job-board-openapi.yml
  format: yaml
  label: Greenhouse Job Board API
  slug: job-board
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-job-board-openapi.yml
- filename: greenhouse-ingestion-openapi.yml
  format: yaml
  label: Greenhouse Candidate Ingestion API
  slug: ingestion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-ingestion-openapi.yml
- filename: greenhouse-onboarding-openapi.yml
  format: yaml
  label: Greenhouse Onboarding API
  slug: onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-onboarding-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Greenhouse Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Greenhouse secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Greenhouse
provider_slug: greenhouse
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/greenhouse-harvest-openapi.yml
  - openapi/greenhouse-ingestion-openapi.yml
  - openapi/greenhouse-job-board-openapi.yml
  - openapi/greenhouse-onboarding-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://api.greenhouse.io/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.greenhouse.io/oauth/token
  name: oauth2
  sources:
  - openapi/greenhouse-ingestion-openapi.yml
  type: oauth2
slug: greenhouse-authentication
source_filename: greenhouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/greenhouse-harvest-openapi.yml, openapi/greenhouse-ingestion-openapi.yml, openapi/greenhouse-job-board-openapi.yml,\n  openapi/greenhouse-onboarding-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/greenhouse-harvest-openapi.yml\n  - openapi/greenhouse-ingestion-openapi.yml\n  - openapi/greenhouse-job-board-openapi.yml\n  - openapi/greenhouse-onboarding-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.greenhouse.io/oauth/authorize\n    tokenUrl: https://api.greenhouse.io/oauth/token\n    scopes: 0\n  sources:\n  - openapi/greenhouse-ingestion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/authentication/greenhouse-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- ATS
- Recruiting
- Candidates
- Jobs
- Onboarding
- HR
---
