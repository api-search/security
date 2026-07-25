---
api_key_in:
- cookie
- header
api_specs:
- filename: authentik-core-api-openapi.yml
  format: yaml
  label: Authentik Core API
  slug: authentik-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-core-api-openapi.yml
- filename: authentik-crypto-api-openapi.yml
  format: yaml
  label: Authentik Crypto API
  slug: authentik-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-crypto-api-openapi.yml
- filename: authentik-events-api-openapi.yml
  format: yaml
  label: Authentik Events API
  slug: authentik-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-events-api-openapi.yml
- filename: authentik-flows-api-openapi.yml
  format: yaml
  label: Authentik Flows API
  slug: authentik-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-flows-api-openapi.yml
- filename: authentik-policies-api-openapi.yml
  format: yaml
  label: Authentik Policies API
  slug: authentik-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-policies-api-openapi.yml
- filename: authentik-providers-api-openapi.yml
  format: yaml
  label: Authentik Providers API
  slug: authentik-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-providers-api-openapi.yml
- filename: authentik-rbac-api-openapi.yml
  format: yaml
  label: Authentik RBAC API
  slug: authentik-rbac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-rbac-api-openapi.yml
- filename: authentik-schema-api-openapi.yml
  format: yaml
  label: Authentik Schema API
  slug: authentik-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-schema-api-openapi.yml
- filename: authentik-sources-api-openapi.yml
  format: yaml
  label: Authentik Sources API
  slug: authentik-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-sources-api-openapi.yml
- filename: authentik-stages-api-openapi.yml
  format: yaml
  label: Authentik Stages API
  slug: authentik-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authentik/refs/heads/main/openapi/authentik-stages-api-openapi.yml
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
