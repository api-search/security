---
api_key_in: []
api_specs:
- filename: trelica-rest-api-openapi.yml
  format: yaml
  label: Trelica REST API
  slug: trelica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trelica/refs/heads/main/openapi/trelica-rest-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Trelica Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Trelica secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Trelica
provider_slug: trelica
scheme_count: 2
schemes:
- description: OAuth 2.0 Client Credentials flow for server-to-server integrations
  flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://app.trelica.com/connect/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/trelica-rest-api-openapi.yml
  type: oauth2
- description: OAuth 2.0 Authorization Code flow for third-party developer apps
  flows:
  - authorizationUrl: https://app.trelica.com/connect/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://app.trelica.com/connect/token
  name: OAuth2AuthorizationCode
  sources:
  - openapi/trelica-rest-api-openapi.yml
  type: oauth2
slug: trelica-authentication
source_filename: trelica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trelica-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.trelica.com/connect/token\n    scopes: 9\n  description: OAuth 2.0 Client Credentials flow for server-to-server integrations\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.trelica.com/connect/authorize\n    tokenUrl: https://app.trelica.com/connect/token\n    scopes: 9\n  description: OAuth 2.0 Authorization Code flow for third-party developer apps\n  sources:\n  - openapi/trelica-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trelica/refs/heads/main/authentication/trelica-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Contract Management
- IT Management
- License Management
- SaaS Management
- Software Asset Management
---
