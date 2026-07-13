---
api_key_in: []
api_specs:
- filename: linode-api-v4-openapi.yml
  format: yaml
  label: Linode API V4
  slug: api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-api-v4-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Linode Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: linode secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: linode
provider_slug: linode
scheme_count: 2
schemes:
- description: A personal access token generated from the Linode Cloud Manager that grants access to the API based on the token's scopes.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/linode-api-v4-openapi.yml
  type: http
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    scopes: 28
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  sources:
  - openapi/linode-api-v4-openapi.yml
  type: oauth2
slug: linode-authentication
source_filename: linode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linode-api-v4-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: A personal access token generated from the Linode Cloud Manager that grants access\n    to the API based on the token's scopes.\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n    scopes: 28\n  description: OAuth 2.0 authentication for third-party applications.\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/authentication/linode-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags: []
---
