---
api_key_in: []
api_specs:
- filename: kings-college-london-altmetric-api-openapi.yml
  format: yaml
  label: King's College London altmetric API
  slug: kings-college-london-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-altmetric-api-openapi.yml
- filename: kings-college-london-articles-api-openapi.yml
  format: yaml
  label: King's College London articles API
  slug: kings-college-london-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-articles-api-openapi.yml
- filename: kings-college-london-authors-api-openapi.yml
  format: yaml
  label: King's College London authors API
  slug: kings-college-london-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-authors-api-openapi.yml
- filename: kings-college-london-collections-api-openapi.yml
  format: yaml
  label: King's College London collections API
  slug: kings-college-london-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-collections-api-openapi.yml
- filename: kings-college-london-institutions-api-openapi.yml
  format: yaml
  label: King's College London institutions API
  slug: kings-college-london-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-institutions-api-openapi.yml
- filename: kings-college-london-oauth-api-openapi.yml
  format: yaml
  label: King's College London oauth API
  slug: kings-college-london-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-oauth-api-openapi.yml
- filename: kings-college-london-other-api-openapi.yml
  format: yaml
  label: King's College London other API
  slug: kings-college-london-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-other-api-openapi.yml
- filename: kings-college-london-profiles-api-openapi.yml
  format: yaml
  label: King's College London profiles API
  slug: kings-college-london-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-profiles-api-openapi.yml
- filename: kings-college-london-projects-api-openapi.yml
  format: yaml
  label: King's College London projects API
  slug: kings-college-london-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-projects-api-openapi.yml
- filename: kings-college-london-symplectic-api-openapi.yml
  format: yaml
  label: King's College London symplectic API
  slug: kings-college-london-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Kings College London Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: King's College London secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: King's College London
provider_slug: kings-college-london
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/kings-college-london-figshare-repository.yaml
  type: oauth2
slug: kings-college-london-authentication
source_filename: kings-college-london-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kings-college-london-figshare-repository.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/kings-college-london-figshare-repository.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/authentication/kings-college-london-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- OAI-PMH
- Library
- United Kingdom
---
