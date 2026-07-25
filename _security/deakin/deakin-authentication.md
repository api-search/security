---
api_key_in: []
api_specs:
- filename: deakin-altmetric-api-openapi.yml
  format: yaml
  label: Deakin University altmetric API
  slug: deakin-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-altmetric-api-openapi.yml
- filename: deakin-articles-api-openapi.yml
  format: yaml
  label: Deakin University articles API
  slug: deakin-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-articles-api-openapi.yml
- filename: deakin-authors-api-openapi.yml
  format: yaml
  label: Deakin University authors API
  slug: deakin-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-authors-api-openapi.yml
- filename: deakin-collections-api-openapi.yml
  format: yaml
  label: Deakin University collections API
  slug: deakin-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-collections-api-openapi.yml
- filename: deakin-institutions-api-openapi.yml
  format: yaml
  label: Deakin University institutions API
  slug: deakin-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-institutions-api-openapi.yml
- filename: deakin-oauth-api-openapi.yml
  format: yaml
  label: Deakin University oauth API
  slug: deakin-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-oauth-api-openapi.yml
- filename: deakin-other-api-openapi.yml
  format: yaml
  label: Deakin University other API
  slug: deakin-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-other-api-openapi.yml
- filename: deakin-profiles-api-openapi.yml
  format: yaml
  label: Deakin University profiles API
  slug: deakin-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-profiles-api-openapi.yml
- filename: deakin-projects-api-openapi.yml
  format: yaml
  label: Deakin University projects API
  slug: deakin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-projects-api-openapi.yml
- filename: deakin-symplectic-api-openapi.yml
  format: yaml
  label: Deakin University symplectic API
  slug: deakin-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Deakin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Deakin University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Deakin University
provider_slug: deakin
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/deakin-figshare-api.yaml
  type: oauth2
slug: deakin-authentication
source_filename: deakin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deakin-figshare-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/deakin-figshare-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/authentication/deakin-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Australia
---
