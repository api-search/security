---
api_key_in: []
api_specs:
- filename: farmos-farmos-api-openapi.yml
  format: yaml
  label: farmOS JSON:API
  slug: farmos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmos/refs/heads/main/openapi/farmos-farmos-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Farmos Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: farmOS secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: farmOS
provider_slug: farmos
scheme_count: 2
schemes:
- description: 'OAuth2 Authorization Code grant for third-party integrations. Users

    authorize the client application to access their farmOS data.'
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: /oauth/token
  name: oauth2AuthorizationCode
  sources:
  - openapi/farmos-farmos-api-openapi.yml
  type: oauth2
- description: 'OAuth2 Client Credentials grant for machine-to-machine authentication.

    Used when no user account is required.'
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: /oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/farmos-farmos-api-openapi.yml
  type: oauth2
slug: farmos-authentication
source_filename: farmos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/farmos-farmos-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2AuthorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n    scopes: 3\n  description: |-\n    OAuth2 Authorization Code grant for third-party integrations. Users\n    authorize the client application to access their farmOS data.\n  sources:\n  - openapi/farmos-farmos-api-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 3\n  description: |-\n    OAuth2 Client Credentials grant for machine-to-machine authentication.\n    Used when no user account is required.\n  sources:\n  - openapi/farmos-farmos-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmos/refs/heads/main/authentication/farmos-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Agriculture
- Farm Management
- Open Source
- JSON:API
- Record Keeping
- Self-Hosted
- Drupal
---
