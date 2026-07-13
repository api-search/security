---
api_key_in: []
api_specs:
- filename: google-artifact-registry-openapi.yml
  format: yaml
  label: Google Artifact Registry
  slug: google-artifact-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-artifact-registry/refs/heads/main/openapi/google-artifact-registry-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Artifact Registry Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Artifact Registry secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Artifact Registry
provider_slug: google-artifact-registry
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-artifact-registry-openapi.yml
  type: oauth2
slug: google-artifact-registry-authentication
source_filename: google-artifact-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-artifact-registry-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/google-artifact-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-artifact-registry/refs/heads/main/authentication/google-artifact-registry-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artifacts
- Containers
- Google Cloud
- Packages
- Registry
---
