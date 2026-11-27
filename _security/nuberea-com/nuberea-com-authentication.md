---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nuberea-com-chat-api-openapi.yml
  format: yaml
  label: nuberea-com Chat API
  slug: nuberea-com-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuberea-com/openapi/nuberea-com-chat-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: nuberea-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: nuberea-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: nuberea-com
provider_slug: nuberea-com
scheme_count: 1
schemes:
- bearerFormat: Firebase ID Token
  description: 'Sign in with your NuBerea account credentials to obtain an ID token. Pass it as `Authorization: Bearer <token>`. Tokens expire after 1 hour. See the Authentication section above for details.'
  name: firebaseAuth
  scheme: bearer
  sources:
  - openapi/nuberea-com-openapi.yml
  type: http
slug: nuberea-com-authentication
source_filename: nuberea-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nuberea-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: firebaseAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Firebase ID Token\n  description: 'Sign in with your NuBerea account credentials to obtain an ID token. Pass it\n    as `Authorization: Bearer <token>`. Tokens expire after 1 hour. See the Authentication section\n    above for details.'\n  sources:\n  - openapi/nuberea-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/nuberea-com/authentication/nuberea-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Bible
- Study
- Theology
- Platform
- Company
---
