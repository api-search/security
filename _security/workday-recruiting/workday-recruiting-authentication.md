---
api_key_in: []
api_specs:
- filename: Recruiting_OpenAPI.yaml
  format: yaml
  label: Workday Recruiting REST API
  slug: workday-recruiting-rest-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Recruiting/v41.2/Recruiting_OpenAPI.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Recruiting Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Workday Recruiting secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Workday Recruiting
provider_slug: workday-recruiting
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication. Register an API client in Workday, grant recruiting scopes, and obtain access tokens.
  flows:
  - authorizationUrl: https://{tenant}.workday.com/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/token
  name: oauth2
  sources:
  - openapi/workday-recruiting-rest-api-openapi.yml
  type: oauth2
slug: workday-recruiting-authentication
source_filename: workday-recruiting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-recruiting-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.workday.com/authorize\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/token\n    scopes: 2\n  description: OAuth 2.0 authentication. Register an API client in Workday, grant recruiting\n    scopes, and obtain access tokens.\n  sources:\n  - openapi/workday-recruiting-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/authentication/workday-recruiting-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HCM
- Human Resources
- Recruiting
- SaaS
- Talent Acquisition
---
