---
api_key_in: []
api_specs:
- filename: hbku-altmetric-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University altmetric API
  slug: hbku-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-altmetric-api-openapi.yml
- filename: hbku-articles-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University articles API
  slug: hbku-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-articles-api-openapi.yml
- filename: hbku-authors-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University authors API
  slug: hbku-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-authors-api-openapi.yml
- filename: hbku-collections-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University collections API
  slug: hbku-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-collections-api-openapi.yml
- filename: hbku-institutions-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University institutions API
  slug: hbku-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-institutions-api-openapi.yml
- filename: hbku-oauth-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University oauth API
  slug: hbku-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-oauth-api-openapi.yml
- filename: hbku-other-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University other API
  slug: hbku-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-other-api-openapi.yml
- filename: hbku-profiles-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University profiles API
  slug: hbku-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-profiles-api-openapi.yml
- filename: hbku-projects-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University projects API
  slug: hbku-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-projects-api-openapi.yml
- filename: hbku-symplectic-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University symplectic API
  slug: hbku-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-symplectic-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hbku Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hamad Bin Khalifa University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hamad Bin Khalifa University
provider_slug: hbku
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/hbku-figshare-api.yaml
  type: oauth2
slug: hbku-authentication
source_filename: hbku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hbku-figshare-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/hbku-figshare-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/authentication/hbku-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Qatar
- Middle East
---
