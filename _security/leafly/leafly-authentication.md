---
api_key_in: []
api_specs:
- filename: leafly-menu-integration-openapi.yml
  format: yaml
  label: Leafly Menu Integration API
  slug: leafly-menu-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leafly/refs/heads/main/openapi/leafly-menu-integration-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Leafly Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Leafly secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Leafly
provider_slug: leafly
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.leafly.com/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/leafly-menu-integration-openapi.yml
  type: oauth2
slug: leafly-authentication
source_filename: leafly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leafly-menu-integration-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.leafly.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/leafly-menu-integration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leafly/refs/heads/main/authentication/leafly-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cannabis
- Dispensary
- Menu Sync
- POS Integration
- Retail
- Marketplace
- Strains
- Ecommerce
---
