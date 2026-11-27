---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-cloud-trace-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Trace Projects API
  slug: google-cloud-trace-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-trace/openapi/google-cloud-trace-projects-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Cloud Trace Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Trace secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Trace
provider_slug: google-cloud-trace
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-cloud-trace-projects-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-cloud-trace-projects-api-openapi.yml
  type: oauth2
slug: google-cloud-trace-authentication
source_filename: google-cloud-trace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-trace-projects-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-cloud-trace-projects-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-cloud-trace-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-trace/authentication/google-cloud-trace-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Distributed Tracing
- Google Cloud
- Latency
- Observability
- Performance
- Spans
- Tracing
---
