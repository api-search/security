---
api_key_in: []
api_specs:
- filename: criteo-openapi.yml
  format: yaml
  label: Criteo Retail Media API
  slug: criteo-retail-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Criteo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Criteo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Criteo
provider_slug: criteo
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.criteo.com/oauth2/token
  - authorizationUrl: https://consent.criteo.com/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.criteo.com/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/criteo-openapi.yml
  type: oauth2
slug: criteo-authentication
source_filename: criteo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/criteo-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://consent.criteo.com/authorize\n    tokenUrl: https://api.criteo.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/criteo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/authentication/criteo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Audiences
- Campaigns
- Catalog
- Commerce
- Display Advertising
- Marketing
- Media
- OAuth 2.0
- Reporting
- Retail
- Retail Media
---
