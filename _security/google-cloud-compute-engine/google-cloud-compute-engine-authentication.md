---
api_key_in: []
api_specs:
- filename: compute-openapi.yml
  format: yaml
  label: Google Compute Engine API
  slug: google-compute-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-compute-engine/refs/heads/main/openapi/compute-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Compute Engine Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Compute Engine secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Compute Engine
provider_slug: google-cloud-compute-engine
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/compute-openapi.yml
  type: oauth2
slug: google-cloud-compute-engine-authentication
source_filename: google-cloud-compute-engine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/compute-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/compute-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-compute-engine/refs/heads/main/authentication/google-cloud-compute-engine-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Compute
- Google Cloud
- IaaS
- Infrastructure
- Virtual Machines
---
