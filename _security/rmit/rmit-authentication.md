---
api_key_in: []
api_specs:
- filename: rmit-altmetric-api-openapi.yml
  format: yaml
  label: RMIT University altmetric API
  slug: rmit-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-altmetric-api-openapi.yml
- filename: rmit-articles-api-openapi.yml
  format: yaml
  label: RMIT University articles API
  slug: rmit-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-articles-api-openapi.yml
- filename: rmit-authors-api-openapi.yml
  format: yaml
  label: RMIT University authors API
  slug: rmit-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-authors-api-openapi.yml
- filename: rmit-collections-api-openapi.yml
  format: yaml
  label: RMIT University collections API
  slug: rmit-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-collections-api-openapi.yml
- filename: rmit-institutions-api-openapi.yml
  format: yaml
  label: RMIT University institutions API
  slug: rmit-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-institutions-api-openapi.yml
- filename: rmit-oauth-api-openapi.yml
  format: yaml
  label: RMIT University oauth API
  slug: rmit-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-oauth-api-openapi.yml
- filename: rmit-other-api-openapi.yml
  format: yaml
  label: RMIT University other API
  slug: rmit-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-other-api-openapi.yml
- filename: rmit-profiles-api-openapi.yml
  format: yaml
  label: RMIT University profiles API
  slug: rmit-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-profiles-api-openapi.yml
- filename: rmit-projects-api-openapi.yml
  format: yaml
  label: RMIT University projects API
  slug: rmit-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-projects-api-openapi.yml
- filename: rmit-symplectic-api-openapi.yml
  format: yaml
  label: RMIT University symplectic API
  slug: rmit-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Rmit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RMIT University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RMIT University
provider_slug: rmit
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/rmit-figshare-api.yaml
  type: oauth2
slug: rmit-authentication
source_filename: rmit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rmit-figshare-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/rmit-figshare-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/authentication/rmit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Australia
---
