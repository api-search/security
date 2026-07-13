---
api_key_in:
- header
api_specs:
- filename: university-of-chicago-fence.yaml
  format: yaml
  label: Gen3 Data Commons APIs (CTDS)
  slug: gen3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-chicago/refs/heads/main/openapi/university-of-chicago-fence.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: University Of Chicago Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: University of Chicago secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: University of Chicago
provider_slug: university-of-chicago
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: /oauth/token
  name: OAuth2
  sources:
  - openapi/university-of-chicago-fence.yaml
  type: oauth2
- name: basic_auth
  scheme: basic
  sources:
  - openapi/university-of-chicago-indexd.yaml
  type: http
- in: header
  name: authToken
  parameter: Authorization
  sources:
  - openapi/university-of-chicago-indexd.yaml
  type: apiKey
slug: university-of-chicago-authentication
source_filename: university-of-chicago-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-chicago-fence.yaml, openapi/university-of-chicago-indexd.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 1\n  sources:\n  - openapi/university-of-chicago-fence.yaml\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/university-of-chicago-indexd.yaml\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/university-of-chicago-indexd.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-chicago/refs/heads/main/authentication/university-of-chicago-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Education
- Higher Education
- University
- Research Data
- Open Source
- IIIF
- Identity
- United States
---
