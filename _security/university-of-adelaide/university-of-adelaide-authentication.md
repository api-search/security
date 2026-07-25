---
api_key_in: []
api_specs:
- filename: university-of-adelaide-altmetric-api-openapi.yml
  format: yaml
  label: University of Adelaide altmetric API
  slug: university-of-adelaide-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-altmetric-api-openapi.yml
- filename: university-of-adelaide-articles-api-openapi.yml
  format: yaml
  label: University of Adelaide articles API
  slug: university-of-adelaide-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-articles-api-openapi.yml
- filename: university-of-adelaide-authors-api-openapi.yml
  format: yaml
  label: University of Adelaide authors API
  slug: university-of-adelaide-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-authors-api-openapi.yml
- filename: university-of-adelaide-collections-api-openapi.yml
  format: yaml
  label: University of Adelaide collections API
  slug: university-of-adelaide-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-collections-api-openapi.yml
- filename: university-of-adelaide-institutions-api-openapi.yml
  format: yaml
  label: University of Adelaide institutions API
  slug: university-of-adelaide-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-institutions-api-openapi.yml
- filename: university-of-adelaide-oauth-api-openapi.yml
  format: yaml
  label: University of Adelaide oauth API
  slug: university-of-adelaide-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-oauth-api-openapi.yml
- filename: university-of-adelaide-other-api-openapi.yml
  format: yaml
  label: University of Adelaide other API
  slug: university-of-adelaide-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-other-api-openapi.yml
- filename: university-of-adelaide-profiles-api-openapi.yml
  format: yaml
  label: University of Adelaide profiles API
  slug: university-of-adelaide-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-profiles-api-openapi.yml
- filename: university-of-adelaide-projects-api-openapi.yml
  format: yaml
  label: University of Adelaide projects API
  slug: university-of-adelaide-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-projects-api-openapi.yml
- filename: university-of-adelaide-symplectic-api-openapi.yml
  format: yaml
  label: University of Adelaide symplectic API
  slug: university-of-adelaide-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: University Of Adelaide Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: University of Adelaide secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: University of Adelaide
provider_slug: university-of-adelaide
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/university-of-adelaide-figshare.yaml
  type: oauth2
slug: university-of-adelaide-authentication
source_filename: university-of-adelaide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-adelaide-figshare.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/university-of-adelaide-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/authentication/university-of-adelaide-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Institutional Repository
- Open Data
- Australia
---
