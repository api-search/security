---
api_key_in: []
api_specs:
- filename: loughborough-altmetric-api-openapi.yml
  format: yaml
  label: Loughborough University altmetric API
  slug: loughborough-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-altmetric-api-openapi.yml
- filename: loughborough-articles-api-openapi.yml
  format: yaml
  label: Loughborough University articles API
  slug: loughborough-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-articles-api-openapi.yml
- filename: loughborough-authors-api-openapi.yml
  format: yaml
  label: Loughborough University authors API
  slug: loughborough-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-authors-api-openapi.yml
- filename: loughborough-collections-api-openapi.yml
  format: yaml
  label: Loughborough University collections API
  slug: loughborough-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-collections-api-openapi.yml
- filename: loughborough-institutions-api-openapi.yml
  format: yaml
  label: Loughborough University institutions API
  slug: loughborough-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-institutions-api-openapi.yml
- filename: loughborough-oauth-api-openapi.yml
  format: yaml
  label: Loughborough University oauth API
  slug: loughborough-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-oauth-api-openapi.yml
- filename: loughborough-other-api-openapi.yml
  format: yaml
  label: Loughborough University other API
  slug: loughborough-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-other-api-openapi.yml
- filename: loughborough-profiles-api-openapi.yml
  format: yaml
  label: Loughborough University profiles API
  slug: loughborough-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-profiles-api-openapi.yml
- filename: loughborough-projects-api-openapi.yml
  format: yaml
  label: Loughborough University projects API
  slug: loughborough-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-projects-api-openapi.yml
- filename: loughborough-symplectic-api-openapi.yml
  format: yaml
  label: Loughborough University symplectic API
  slug: loughborough-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Loughborough Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Loughborough University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Loughborough University
provider_slug: loughborough
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/loughborough-research-repository-rest.yaml
  type: oauth2
slug: loughborough-authentication
source_filename: loughborough-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loughborough-research-repository-rest.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/loughborough-research-repository-rest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/authentication/loughborough-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research Data
- Open Access
- Repository
- Identity
---
