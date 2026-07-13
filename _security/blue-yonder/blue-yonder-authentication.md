---
api_key_in: []
api_specs:
- filename: blue-yonder-warehouse-management-openapi.yml
  format: yaml
  label: Blue Yonder Warehouse Management API
  slug: blue-yonder-warehouse-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/openapi/blue-yonder-warehouse-management-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Blue Yonder Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: blue-yonder secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: blue-yonder
provider_slug: blue-yonder
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.blueyonder.example.com/oauth/token
  name: oauth2
  sources:
  - openapi/blue-yonder-warehouse-management-openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blue-yonder-warehouse-management-openapi.yml
  type: http
slug: blue-yonder-authentication
source_filename: blue-yonder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blue-yonder-warehouse-management-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.blueyonder.example.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/blue-yonder-warehouse-management-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/blue-yonder-warehouse-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/authentication/blue-yonder-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags: []
---
