---
api_key_in: []
api_specs:
- filename: mojang-public-api-openapi.yml
  format: yaml
  label: Mojang Public API
  slug: mojang-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-public-api-openapi.yml
- filename: mojang-session-server-openapi.yml
  format: yaml
  label: Mojang Session Server
  slug: mojang-session-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-session-server-openapi.yml
- filename: mojang-minecraft-services-openapi.yml
  format: yaml
  label: Minecraft Services API
  slug: minecraft-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-minecraft-services-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mojang Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mojang secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mojang
provider_slug: mojang
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Minecraft access token issued by /authentication/login_with_xbox. Used as `Authorization: Bearer {token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mojang-minecraft-services-openapi.yml
  - openapi/mojang-session-server-openapi.yml
  type: http
slug: mojang-authentication
source_filename: mojang-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mojang-minecraft-services-openapi.yml, openapi/mojang-session-server-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Minecraft access token issued by /authentication/login_with_xbox. Used as `Authorization:\n    Bearer {token}`.'\n  sources:\n  - openapi/mojang-minecraft-services-openapi.yml\n  - openapi/mojang-session-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/authentication/mojang-authentication.yml
summary_line: http · 1 scheme
tags:
- Games And Comics
- Minecraft
- Gaming
- Identity
- Player Profiles
- Session
- Public APIs
---
