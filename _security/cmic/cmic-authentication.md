---
api_key_in: []
api_specs:
- filename: cmic-construction-erp-openapi.yml
  format: yaml
  label: CMiC Construction ERP API
  slug: cmic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cmic/refs/heads/main/openapi/cmic-construction-erp-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cmic Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CMiC secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CMiC
provider_slug: cmic
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials for CMiC API access
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/cmic-construction-erp-openapi.yml
  type: oauth2
slug: cmic-authentication
source_filename: cmic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cmic-construction-erp-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: OAuth 2.0 client credentials for CMiC API access\n  sources:\n  - openapi/cmic-construction-erp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cmic/refs/heads/main/authentication/cmic-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Construction
- ERP
- Finance
- Project Management
---
