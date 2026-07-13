---
api_key_in: []
api_specs:
- filename: cloud-spanner-openapi.yml
  format: yaml
  label: Cloud Spanner API
  slug: cloud-spanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-spanner/refs/heads/main/openapi/cloud-spanner-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Cloud Spanner Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Cloud Spanner secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Cloud Spanner
provider_slug: google-cloud-spanner
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/cloud-spanner-openapi.yml
  type: oauth2
slug: google-cloud-spanner-authentication
source_filename: google-cloud-spanner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-spanner-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/cloud-spanner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-spanner/refs/heads/main/authentication/google-cloud-spanner-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Database
- Distributed
- Google Cloud
- Relational
- SQL
---
