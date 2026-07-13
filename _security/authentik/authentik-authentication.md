---
api_key_in:
- cookie
- header
api_specs:
- filename: schema_retrieve
  format: yaml
  label: Authentik REST API
  slug: authentik-rest-api
  spec_type: OpenAPI
  url: https://api.goauthentik.io/#/Schema/schema_retrieve
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Authentik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Authentik secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Authentik
provider_slug: authentik
scheme_count: 2
schemes:
- description: 'authentik token authentication. Use header

    `Authorization: Bearer <token>` with a token created in the

    Tokens & App Passwords section.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/authentik-openapi.yml
  type: apiKey
- description: Browser session cookie for interactive use.
  in: cookie
  name: sessionAuth
  parameter: authentik_session
  sources:
  - openapi/authentik-openapi.yml
  type: apiKey
slug: authentik-authentication
source_filename: authentik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/authentik-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    authentik token authentication. Use header\n    `Authorization: Bearer <token>` with a token created in the\n    Tokens & App Passwords section.\n  sources:\n  - openapi/authentik-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  parameter: authentik_session\n  description: Browser session cookie for interactive use.\n  sources:\n  - openapi/authentik-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/authentication/authentik-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Authentication
- Authorization
- Identity Provider
- LDAP
- OAuth
- Open Source
- OpenID Connect
- SAML
- SCIM
- Self-Hosted
---
