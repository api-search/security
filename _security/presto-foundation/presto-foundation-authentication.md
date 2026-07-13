---
api_key_in: []
api_specs:
- filename: presto-foundation-openapi.yml
  format: yaml
  label: Presto Client REST API
  slug: presto-client-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/openapi/presto-foundation-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Presto Foundation Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Presto Foundation secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Presto Foundation
provider_slug: presto-foundation
scheme_count: 2
schemes:
- description: Basic auth, typically used with LDAP or password-file authenticators.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/presto-foundation-openapi.yml
  type: http
- description: OAuth 2.0 authenticator (when enabled on the coordinator).
  flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://example.com/oauth/token
  name: oauth2
  sources:
  - openapi/presto-foundation-openapi.yml
  type: oauth2
slug: presto-foundation-authentication
source_filename: presto-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/presto-foundation-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic auth, typically used with LDAP or password-file authenticators.\n  sources:\n  - openapi/presto-foundation-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authenticator (when enabled on the coordinator).\n  sources:\n  - openapi/presto-foundation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/authentication/presto-foundation-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Analytics
- Big Data
- Distributed SQL
- Linux Foundation
- Open Source
- Query Engine
- SQL
---
