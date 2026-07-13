---
api_key_in: []
api_specs:
- filename: majesco-policy-openapi.yml
  format: yaml
  label: Majesco Insurance SaaS API
  slug: majesco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/majesco/refs/heads/main/openapi/majesco-policy-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Majesco Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: majesco secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: majesco
provider_slug: majesco
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.majesco.example.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/majesco-policy-openapi.yml
  type: oauth2
slug: majesco-authentication
source_filename: majesco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/majesco-policy-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.majesco.example.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/majesco-policy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/majesco/refs/heads/main/authentication/majesco-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
