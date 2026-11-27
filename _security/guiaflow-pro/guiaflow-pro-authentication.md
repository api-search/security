---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GuiaFlow Authentication
name_suffix: Authentication
oauth_flows: []
overview: GuiaFlow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GuiaFlow
provider_slug: guiaflow-pro
scheme_count: 1
schemes:
- description: Chave pessoal gf_live_… (Conta → Chaves de API) ou token OAuth.
  name: bearer
  scheme: bearer
  sources:
  - openapi/guiaflow-pro-openapi.json
  type: http
slug: guiaflow-pro-authentication
source_filename: guiaflow-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/guiaflow-pro-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Chave pessoal gf_live_… (Conta → Chaves de API) ou token OAuth.\n  sources:\n  - openapi/guiaflow-pro-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/guiaflow-pro/authentication/guiaflow-pro-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Interactive
- Demo
- No-Code
- Artificial Intelligence
---
