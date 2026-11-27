---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: maketa-pro-agent-api-openapi.yml
  format: yaml
  label: Maketa Agent API
  slug: maketa-pro-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-agent-api-openapi.yml
- filename: maketa-pro-boards-api-openapi.yml
  format: yaml
  label: Maketa Boards API
  slug: maketa-pro-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-boards-api-openapi.yml
- filename: maketa-pro-keys-api-openapi.yml
  format: yaml
  label: Maketa Keys API
  slug: maketa-pro-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-keys-api-openapi.yml
- filename: maketa-pro-misc-api-openapi.yml
  format: yaml
  label: Maketa Misc API
  slug: maketa-pro-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-misc-api-openapi.yml
- filename: maketa-pro-screens-api-openapi.yml
  format: yaml
  label: Maketa Screens API
  slug: maketa-pro-screens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-screens-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Maketa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maketa secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Maketa
provider_slug: maketa-pro
scheme_count: 3
schemes:
- description: Песочный ключ агента mk_sb_… (POST /agent/register) или проектный ключ доски mk_pk_… (POST /project/key).
  in: header
  name: maketaKey
  parameter: x-maketa-key
  sources:
  - openapi/maketa-pro-openapi.json
  type: apiKey
- description: Секретный edit-токен доски из ответа POST /create (в POST-ручках передаётся полем edit в теле).
  in: query
  name: editToken
  parameter: edit
  sources:
  - openapi/maketa-pro-openapi.json
  type: apiKey
- description: OAuth 2.1 access-токен, либо непосредственно ключ mk_pk_/mk_sb_.
  name: mcpBearer
  scheme: bearer
  sources:
  - openapi/maketa-pro-openapi.json
  type: http
slug: maketa-pro-authentication
source_filename: maketa-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/maketa-pro-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: maketaKey\n  type: apiKey\n  in: header\n  parameter: x-maketa-key\n  description: Песочный ключ агента mk_sb_… (POST /agent/register) или проектный ключ доски\n    mk_pk_… (POST /project/key).\n  sources:\n  - openapi/maketa-pro-openapi.json\n- name: editToken\n  type: apiKey\n  in: query\n  parameter: edit\n  description: Секретный edit-токен доски из ответа POST /create (в POST-ручках передаётся полем\n    edit в теле).\n  sources:\n  - openapi/maketa-pro-openapi.json\n- name: mcpBearer\n  type: http\n  scheme: bearer\n  description: OAuth 2.1 access-токен, либо непосредственно ключ mk_pk_/mk_sb_.\n  sources:\n  - openapi/maketa-pro-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/maketa-pro/authentication/maketa-pro-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- No-Code
- Prototyping
- Screen-Constructor
- AI-assisted
- Mockup
---
