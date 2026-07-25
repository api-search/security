---
api_key_in: []
api_specs:
- filename: monash-altmetric-api-openapi.yml
  format: yaml
  label: Monash University altmetric API
  slug: monash-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-altmetric-api-openapi.yml
- filename: monash-articles-api-openapi.yml
  format: yaml
  label: Monash University articles API
  slug: monash-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-articles-api-openapi.yml
- filename: monash-authors-api-openapi.yml
  format: yaml
  label: Monash University authors API
  slug: monash-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-authors-api-openapi.yml
- filename: monash-collections-api-openapi.yml
  format: yaml
  label: Monash University collections API
  slug: monash-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-collections-api-openapi.yml
- filename: monash-institutions-api-openapi.yml
  format: yaml
  label: Monash University institutions API
  slug: monash-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-institutions-api-openapi.yml
- filename: monash-oauth-api-openapi.yml
  format: yaml
  label: Monash University oauth API
  slug: monash-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-oauth-api-openapi.yml
- filename: monash-other-api-openapi.yml
  format: yaml
  label: Monash University other API
  slug: monash-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-other-api-openapi.yml
- filename: monash-profiles-api-openapi.yml
  format: yaml
  label: Monash University profiles API
  slug: monash-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-profiles-api-openapi.yml
- filename: monash-projects-api-openapi.yml
  format: yaml
  label: Monash University projects API
  slug: monash-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-projects-api-openapi.yml
- filename: monash-symplectic-api-openapi.yml
  format: yaml
  label: Monash University symplectic API
  slug: monash-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Monash Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Monash University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Monash University
provider_slug: monash
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/monash-figshare.yaml
  type: oauth2
slug: monash-authentication
source_filename: monash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/monash-figshare.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/monash-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/authentication/monash-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Australia
---
