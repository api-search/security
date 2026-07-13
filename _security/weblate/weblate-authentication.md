---
api_key_in:
- cookie
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Weblate REST API
  slug: weblate-rest-api
  spec_type: OpenAPI
  url: https://hosted.weblate.org/api/schema/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Weblate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weblate secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Weblate
provider_slug: weblate
scheme_count: 3
schemes:
- description: 'Token-based authentication with required prefix `Bearer`.


    - Each user has a personal access token which they can get from their respective user profile. These tokens have the `wlu_` prefix.

    - It is possible to create project tokens whose access to the API is limited to operations to their associated project. These tokens have the `wlp_` prefix.'
  in: header
  name: bearerAuth
  parameter: Bearer
  sources:
  - openapi/weblate-weblate-rest-api-openapi.yml
  type: apiKey
- description: Session-based authentication used when user is signed in.
  in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/weblate-weblate-rest-api-openapi.yml
  type: apiKey
- description: 'Token-based authentication with required prefix `Token`.


    - Each user has a personal access token which they can get from their respective user profile. These tokens have the `wlu_` prefix.

    - It is possible to create project tokens whose access to the API is limited to operations to their associated project. These tokens have the `wlp_` prefix.'
  in: header
  name: tokenAuth
  parameter: Token
  sources:
  - openapi/weblate-weblate-rest-api-openapi.yml
  type: apiKey
slug: weblate-authentication
source_filename: weblate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weblate-weblate-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Bearer\n  description: |-\n    Token-based authentication with required prefix `Bearer`.\n\n    - Each user has a personal access token which they can get from their respective user profile. These tokens have the `wlu_` prefix.\n    - It is possible to create project tokens whose access to the API is limited to operations to their associated project. These tokens have the `wlp_` prefix.\n  sources:\n  - openapi/weblate-weblate-rest-api-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  description: Session-based authentication used when user is signed in.\n  sources:\n  - openapi/weblate-weblate-rest-api-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Token\n  description: |-\n\
  \    Token-based authentication with required prefix `Token`.\n\n    - Each user has a personal access token which they can get from their respective user profile. These tokens have the `wlu_` prefix.\n    - It is possible to create project tokens whose access to the API is limited to operations to their associated project. These tokens have the `wlp_` prefix.\n  sources:\n  - openapi/weblate-weblate-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weblate/refs/heads/main/authentication/weblate-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Localization
- Translation
- Internationalization
- Open Source
- Continuous Localization
- Version Control
---
