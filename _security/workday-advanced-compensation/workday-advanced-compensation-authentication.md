---
api_key_in: []
api_specs:
- filename: Compensation.yaml
  format: yaml
  label: Workday Advanced Compensation API
  slug: workday-advanced-compensation-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Compensation/v41.1/Compensation.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Advanced Compensation Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Workday Advanced Compensation secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Workday Advanced Compensation
provider_slug: workday-advanced-compensation
scheme_count: 1
schemes:
- description: Workday OAuth 2.0 authentication
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  sources:
  - openapi/workday-advanced-compensation-openapi.yml
  type: oauth2
slug: workday-advanced-compensation-authentication
source_filename: workday-advanced-compensation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-advanced-compensation-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n    scopes: 2\n  description: Workday OAuth 2.0 authentication\n  sources:\n  - openapi/workday-advanced-compensation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/authentication/workday-advanced-compensation-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
