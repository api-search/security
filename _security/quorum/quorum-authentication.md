---
api_key_in: []
api_specs:
- filename: quorum-land-management-openapi.yml
  format: yaml
  label: Quorum Land Management API
  slug: quorum-land-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-land-management-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Quorum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Quorum Software secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Quorum Software
provider_slug: quorum
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.quorumsoftware.com/oauth2/token
  name: oauth2
  sources:
  - openapi/quorum-land-management-openapi.yml
  type: oauth2
slug: quorum-authentication
source_filename: quorum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quorum-land-management-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.quorumsoftware.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/quorum-land-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/authentication/quorum-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Energy
- Oil & Gas
- Upstream
- Land Management
- Royalty Accounting
- Production Reporting
---
