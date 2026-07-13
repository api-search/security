---
api_key_in: []
api_specs:
- filename: pg-and-e-share-my-data-api-openapi.yml
  format: yaml
  label: PG&E Share My Data API
  slug: share-my-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-share-my-data-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pg And E Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: pg-and-e secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: pg-and-e
provider_slug: pg-and-e
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.pge.com/datacustodian/oauth/v2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token
  name: oauth2
  sources:
  - openapi/pg-and-e-share-my-data-api-openapi.yml
  type: oauth2
slug: pg-and-e-authentication
source_filename: pg-and-e-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pg-and-e-share-my-data-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.pge.com/datacustodian/oauth/v2/authorize\n    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token\n    scopes: 1\n  sources:\n  - openapi/pg-and-e-share-my-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/authentication/pg-and-e-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
