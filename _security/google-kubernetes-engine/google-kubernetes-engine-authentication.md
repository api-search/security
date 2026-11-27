---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-kubernetes-engine-projects-api-openapi.yml
  format: yaml
  label: Google Kubernetes Engine Projects API
  slug: google-kubernetes-engine-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-kubernetes-engine/openapi/google-kubernetes-engine-projects-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Kubernetes Engine Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Kubernetes Engine secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Kubernetes Engine
provider_slug: google-kubernetes-engine
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-kubernetes-engine-container-projects-api-openapi.yml
  - openapi/google-kubernetes-engine-gkebackup-projects-api-openapi.yml
  - openapi/google-kubernetes-engine-gkehub-projects-api-openapi.yml
  - openapi/google-kubernetes-engine-gkeonprem-projects-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-kubernetes-engine-container-projects-api-openapi.yml
  - openapi/google-kubernetes-engine-gkebackup-projects-api-openapi.yml
  - openapi/google-kubernetes-engine-gkehub-projects-api-openapi.yml
  - openapi/google-kubernetes-engine-gkeonprem-projects-api-openapi.yml
  type: oauth2
slug: google-kubernetes-engine-authentication
source_filename: google-kubernetes-engine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-kubernetes-engine-container-projects-api-openapi.yml, openapi/google-kubernetes-engine-gkebackup-projects-api-openapi.yml,\n  openapi/google-kubernetes-engine-gkehub-projects-api-openapi.yml, openapi/google-kubernetes-engine-gkeonprem-projects-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-kubernetes-engine-container-projects-api-openapi.yml\n  - openapi/google-kubernetes-engine-gkebackup-projects-api-openapi.yml\n  - openapi/google-kubernetes-engine-gkehub-projects-api-openapi.yml\n  - openapi/google-kubernetes-engine-gkeonprem-projects-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n\
  \    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/google-kubernetes-engine-container-projects-api-openapi.yml\n  - openapi/google-kubernetes-engine-gkebackup-projects-api-openapi.yml\n  - openapi/google-kubernetes-engine-gkehub-projects-api-openapi.yml\n  - openapi/google-kubernetes-engine-gkeonprem-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-kubernetes-engine/authentication/google-kubernetes-engine-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Cloud-Native
- Containers
- Google Cloud
- Kubernetes
- Managed Service
- Container Orchestration
---
