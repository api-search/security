---
api_key_in: []
api_specs:
- filename: taylors-library-rest.yaml
  format: yaml
  label: Taylor's Library Koha REST API
  slug: library-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-library-rest.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Taylors Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Taylor's University secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Taylor's University
provider_slug: taylors
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/taylors-library-rest.yaml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/taylors-library-rest.yaml
  type: oauth2
slug: taylors-authentication
source_filename: taylors-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taylors-library-rest.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/taylors-library-rest.yaml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/taylors-library-rest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/authentication/taylors-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Education
- Higher Education
- University
- Library
- Institutional Repository
- Open Data
- Malaysia
- Asia
---
