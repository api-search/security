---
api_key_in:
- header
api_specs:
- filename: ory-hydra-openapi.json
  format: json
  label: Ory Hydra
  slug: hydra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-hydra-openapi.json
- filename: ory-kratos-openapi.json
  format: json
  label: Ory Kratos
  slug: kratos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-kratos-openapi.json
- filename: ory-keto-openapi.json
  format: json
  label: Ory Keto
  slug: keto
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-keto-openapi.json
- filename: ory-oathkeeper-openapi.json
  format: json
  label: Ory Oathkeeper
  slug: oathkeeper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-oathkeeper-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ory Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ory secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ory
provider_slug: ory
scheme_count: 4
schemes:
- name: basic
  scheme: basic
  sources:
  - openapi/ory-hydra-openapi.json
  type: http
- name: bearer
  scheme: bearer
  sources:
  - openapi/ory-hydra-openapi.json
  type: http
- flows:
  - authorizationUrl: https://hydra.demo.ory.sh/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://hydra.demo.ory.sh/oauth2/token
  name: oauth2
  sources:
  - openapi/ory-hydra-openapi.json
  type: oauth2
- in: header
  name: oryAccessToken
  parameter: Authorization
  sources:
  - openapi/ory-kratos-openapi.json
  type: apiKey
slug: ory-authentication
source_filename: ory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ory-hydra-openapi.json, openapi/ory-kratos-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/ory-hydra-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ory-hydra-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hydra.demo.ory.sh/oauth2/auth\n    tokenUrl: https://hydra.demo.ory.sh/oauth2/token\n    scopes: 3\n  sources:\n  - openapi/ory-hydra-openapi.json\n- name: oryAccessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/ory-kratos-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/authentication/ory-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Authentication
- Authorization
- Identity
- OAuth2
- OpenID Connect
- Open Source
---
