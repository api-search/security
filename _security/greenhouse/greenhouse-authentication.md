---
api_key_in: []
api_specs:
- filename: greenhouse-applications-api-openapi.yml
  format: yaml
  label: Greenhouse Applications API
  slug: greenhouse-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-applications-api-openapi.yml
- filename: greenhouse-candidates-api-openapi.yml
  format: yaml
  label: Greenhouse Candidates API
  slug: greenhouse-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-candidates-api-openapi.yml
- filename: greenhouse-departments-api-openapi.yml
  format: yaml
  label: Greenhouse Departments API
  slug: greenhouse-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-departments-api-openapi.yml
- filename: greenhouse-education-api-openapi.yml
  format: yaml
  label: Greenhouse Education API
  slug: greenhouse-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-education-api-openapi.yml
- filename: greenhouse-graphql-api-openapi.yml
  format: yaml
  label: Greenhouse Graphql API
  slug: greenhouse-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-graphql-api-openapi.yml
- filename: greenhouse-greenhouse-job-board-api-api-openapi.yml
  format: yaml
  label: Greenhouse Greenhouse Job Board API API
  slug: greenhouse-greenhouse-job-board-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-greenhouse-job-board-api-api-openapi.yml
- filename: greenhouse-jobs-api-openapi.yml
  format: yaml
  label: Greenhouse Jobs API
  slug: greenhouse-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-jobs-api-openapi.yml
- filename: greenhouse-offices-api-openapi.yml
  format: yaml
  label: Greenhouse Offices API
  slug: greenhouse-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-offices-api-openapi.yml
- filename: greenhouse-prospects-api-openapi.yml
  format: yaml
  label: Greenhouse Prospects API
  slug: greenhouse-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-prospects-api-openapi.yml
- filename: greenhouse-sections-api-openapi.yml
  format: yaml
  label: Greenhouse Sections API
  slug: greenhouse-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-sections-api-openapi.yml
- filename: greenhouse-tracking-api-openapi.yml
  format: yaml
  label: Greenhouse Tracking API
  slug: greenhouse-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-tracking-api-openapi.yml
- filename: greenhouse-users-api-openapi.yml
  format: yaml
  label: Greenhouse Users API
  slug: greenhouse-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-users-api-openapi.yml
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
- Job
- Onboarding
- HR
---
