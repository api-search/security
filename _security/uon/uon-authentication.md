---
api_key_in: []
api_specs:
- filename: uon-altmetric-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia altmetric API
  slug: uon-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-altmetric-api-openapi.yml
- filename: uon-articles-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia articles API
  slug: uon-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-articles-api-openapi.yml
- filename: uon-authors-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia authors API
  slug: uon-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-authors-api-openapi.yml
- filename: uon-collections-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia collections API
  slug: uon-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-collections-api-openapi.yml
- filename: uon-institutions-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia institutions API
  slug: uon-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-institutions-api-openapi.yml
- filename: uon-oauth-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia oauth API
  slug: uon-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-oauth-api-openapi.yml
- filename: uon-other-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia other API
  slug: uon-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-other-api-openapi.yml
- filename: uon-profiles-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia profiles API
  slug: uon-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-profiles-api-openapi.yml
- filename: uon-projects-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia projects API
  slug: uon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-projects-api-openapi.yml
- filename: uon-symplectic-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia symplectic API
  slug: uon-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Uon Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: University of Newcastle Australia secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: University of Newcastle Australia
provider_slug: uon
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/uon-open-research-figshare.yaml
  type: oauth2
slug: uon-authentication
source_filename: uon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uon-open-research-figshare.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/uon-open-research-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/authentication/uon-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Research
- Open Access
- Repository
- OAI-PMH
- Australia
---
