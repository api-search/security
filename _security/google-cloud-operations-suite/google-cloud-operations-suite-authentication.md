---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-cloud-operations-suite-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Operations Suite Projects API
  slug: google-cloud-operations-suite-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-operations-suite/openapi/google-cloud-operations-suite-projects-api-openapi.yml
- filename: google-cloud-operations-suite-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Observability Cloud Operations Suite Folders API
  slug: google-cloud-operations-suite-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-operations-suite/openapi/google-cloud-operations-suite-folders-api-openapi.yml
- filename: google-cloud-operations-suite-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Observability Cloud Operations Suite Organizations API
  slug: google-cloud-operations-suite-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-operations-suite/openapi/google-cloud-operations-suite-organizations-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Cloud Observability Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Observability secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Observability
provider_slug: google-cloud-operations-suite
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-cloud-operations-suite-folders-api-openapi.yml
  - openapi/google-cloud-operations-suite-organizations-api-openapi.yml
  - openapi/google-cloud-operations-suite-projects-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-cloud-operations-suite-folders-api-openapi.yml
  - openapi/google-cloud-operations-suite-organizations-api-openapi.yml
  - openapi/google-cloud-operations-suite-projects-api-openapi.yml
  type: oauth2
slug: google-cloud-operations-suite-authentication
source_filename: google-cloud-operations-suite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-operations-suite-folders-api-openapi.yml, openapi/google-cloud-operations-suite-organizations-api-openapi.yml,\n  openapi/google-cloud-operations-suite-projects-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-cloud-operations-suite-folders-api-openapi.yml\n  - openapi/google-cloud-operations-suite-organizations-api-openapi.yml\n  - openapi/google-cloud-operations-suite-projects-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/google-cloud-operations-suite-folders-api-openapi.yml\n\
  \  - openapi/google-cloud-operations-suite-organizations-api-openapi.yml\n  - openapi/google-cloud-operations-suite-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-operations-suite/authentication/google-cloud-operations-suite-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Error Reporting
- Google Cloud
- Logging
- Monitoring
- Observability
- Profiling
- Stackdriver
- Tracing
---
