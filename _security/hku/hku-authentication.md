---
api_key_in: []
api_specs:
- filename: hku-altmetric-api-openapi.yml
  format: yaml
  label: University of Hong Kong altmetric API
  slug: hku-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-altmetric-api-openapi.yml
- filename: hku-articles-api-openapi.yml
  format: yaml
  label: University of Hong Kong articles API
  slug: hku-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-articles-api-openapi.yml
- filename: hku-authors-api-openapi.yml
  format: yaml
  label: University of Hong Kong authors API
  slug: hku-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-authors-api-openapi.yml
- filename: hku-collections-api-openapi.yml
  format: yaml
  label: University of Hong Kong collections API
  slug: hku-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-collections-api-openapi.yml
- filename: hku-institutions-api-openapi.yml
  format: yaml
  label: University of Hong Kong institutions API
  slug: hku-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-institutions-api-openapi.yml
- filename: hku-oauth-api-openapi.yml
  format: yaml
  label: University of Hong Kong oauth API
  slug: hku-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-oauth-api-openapi.yml
- filename: hku-other-api-openapi.yml
  format: yaml
  label: University of Hong Kong other API
  slug: hku-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-other-api-openapi.yml
- filename: hku-profiles-api-openapi.yml
  format: yaml
  label: University of Hong Kong profiles API
  slug: hku-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-profiles-api-openapi.yml
- filename: hku-projects-api-openapi.yml
  format: yaml
  label: University of Hong Kong projects API
  slug: hku-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-projects-api-openapi.yml
- filename: hku-symplectic-api-openapi.yml
  format: yaml
  label: University of Hong Kong symplectic API
  slug: hku-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hku Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: University of Hong Kong secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: University of Hong Kong
provider_slug: hku
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/hku-datahub.yaml
  type: oauth2
slug: hku-authentication
source_filename: hku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hku-datahub.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/hku-datahub.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/authentication/hku-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Hong Kong
---
