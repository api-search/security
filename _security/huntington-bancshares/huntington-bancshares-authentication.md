---
api_key_in: []
api_specs:
- filename: huntington-bank-treasury-management-api-openapi.yml
  format: yaml
  label: Huntington Bank Treasury Management API
  slug: treasury-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntington-bancshares/refs/heads/main/openapi/huntington-bank-treasury-management-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Huntington Bancshares Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Huntington Bancshares secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Huntington Bancshares
provider_slug: huntington-bancshares
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.huntington.com/oauth/token
  name: oauth2
  sources:
  - openapi/huntington-bank-treasury-management-api-openapi.yml
  type: oauth2
slug: huntington-bancshares-authentication
source_filename: huntington-bancshares-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/huntington-bank-treasury-management-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.huntington.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/huntington-bank-treasury-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntington-bancshares/refs/heads/main/authentication/huntington-bancshares-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking
- ERP Integration
- Open Banking
- Payments
- Treasury
- Fortune 1000
---
