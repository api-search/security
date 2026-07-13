---
api_key_in: []
api_specs:
- filename: greenhouse-harvest-api-openapi.yml
  format: yaml
  label: Greenhouse Harvest API
  slug: greenhouse-harvest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-harvest-api-openapi.yml
- filename: greenhouse-job-board-api-openapi.yml
  format: yaml
  label: Greenhouse Job Board API
  slug: greenhouse-job-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-job-board-api-openapi.yml
- filename: greenhouse-audit-log-api-openapi.yml
  format: yaml
  label: Greenhouse Audit Log API
  slug: greenhouse-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-audit-log-api-openapi.yml
- filename: greenhouse-candidate-ingestion-api-openapi.yml
  format: yaml
  label: Greenhouse Candidate Ingestion (Partner) API
  slug: greenhouse-candidate-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-candidate-ingestion-api-openapi.yml
- filename: greenhouse-onboarding-api-openapi.yml
  format: yaml
  label: Greenhouse Onboarding API
  slug: greenhouse-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-onboarding-api-openapi.yml
- filename: greenhouse-assessment-api-openapi.yml
  format: yaml
  label: Greenhouse Assessment Partner API
  slug: greenhouse-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/openapi/greenhouse-assessment-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Greenhouse Io Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Greenhouse secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Greenhouse
provider_slug: greenhouse-io
scheme_count: 3
schemes:
- description: HTTP Basic; the API key is Base64-encoded and used as the username (key must be <171 chars).
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/greenhouse-assessment-api-openapi.yml
  - openapi/greenhouse-audit-log-api-openapi.yml
  - openapi/greenhouse-candidate-ingestion-api-openapi.yml
  - openapi/greenhouse-harvest-api-openapi.yml
  - openapi/greenhouse-job-board-api-openapi.yml
  - openapi/greenhouse-onboarding-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/greenhouse-audit-log-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://app.greenhouse.io/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://app.greenhouse.io/oauth/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://app.greenhouse.io/oauth/token
  name: OAuth2
  sources:
  - openapi/greenhouse-candidate-ingestion-api-openapi.yml
  type: oauth2
slug: greenhouse-io-authentication
source_filename: greenhouse-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/greenhouse-assessment-api-openapi.yml, openapi/greenhouse-audit-log-api-openapi.yml,\n  openapi/greenhouse-candidate-ingestion-api-openapi.yml, openapi/greenhouse-harvest-api-openapi.yml,\n  openapi/greenhouse-job-board-api-openapi.yml, openapi/greenhouse-onboarding-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic; the API key is Base64-encoded and used as the username (key must\n    be <171 chars).\n  sources:\n  - openapi/greenhouse-assessment-api-openapi.yml\n  - openapi/greenhouse-audit-log-api-openapi.yml\n  - openapi/greenhouse-candidate-ingestion-api-openapi.yml\n  - openapi/greenhouse-harvest-api-openapi.yml\n  - openapi/greenhouse-job-board-api-openapi.yml\n  - openapi/greenhouse-onboarding-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n\
  \  bearerFormat: JWT\n  sources:\n  - openapi/greenhouse-audit-log-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.greenhouse.io/oauth/authorize\n    tokenUrl: https://app.greenhouse.io/oauth/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://app.greenhouse.io/oauth/token\n    scopes: 1\n  sources:\n  - openapi/greenhouse-candidate-ingestion-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/authentication/greenhouse-io-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- ATS
- Recruiting
- Hiring
- Talent Acquisition
- Enterprise SaaS
- Human Resources
- Onboarding
---
