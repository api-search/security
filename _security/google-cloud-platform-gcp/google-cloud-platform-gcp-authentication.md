---
api_key_in: []
api_specs:
- filename: google-cloud-platform-gcp-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Projects API
  slug: google-cloud-platform-gcp-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform-gcp/refs/heads/main/openapi/google-cloud-platform-gcp-projects-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Platform Gcp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Platform secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform-gcp
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-cloud-platform-gcp-openapi.yml
  type: oauth2
slug: google-cloud-platform-gcp-authentication
source_filename: google-cloud-platform-gcp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-cloud-platform-gcp-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-cloud-platform-gcp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform-gcp/refs/heads/main/authentication/google-cloud-platform-gcp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Computing
- Data Analytics
- Infrastructure-as-a-Service
- Machine-Learning
- Platform-as-a-Service
- Software-as-a-Service
- Serverless
---
