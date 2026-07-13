---
api_key_in: []
api_specs:
- filename: allianz-api-connect.yaml
  format: yaml
  label: Allianz API Connect
  slug: allianz-api-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/openapi/allianz-api-connect.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Allianz Docs Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Allianz secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Allianz
provider_slug: allianz-docs
scheme_count: 1
schemes:
- description: OAuth2 client credentials flow for partner API access
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://api.allianz.com.au/oauth2/token
  name: OAuth2
  sources:
  - openapi/allianz-api-connect.yaml
  type: oauth2
slug: allianz-docs-authentication
source_filename: allianz-docs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-api-connect.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.allianz.com.au/oauth2/token\n    scopes: 4\n  description: OAuth2 client credentials flow for partner API access\n  sources:\n  - openapi/allianz-api-connect.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/authentication/allianz-docs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Financial Services
- Insurance
- Asset Management
---
