---
api_key_in: []
api_specs:
- filename: mojang-attributes-api-openapi.yml
  format: yaml
  label: Mojang Attributes API
  slug: mojang-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-attributes-api-openapi.yml
- filename: mojang-authentication-api-openapi.yml
  format: yaml
  label: Mojang Authentication API
  slug: mojang-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-authentication-api-openapi.yml
- filename: mojang-blocklist-api-openapi.yml
  format: yaml
  label: Mojang Blocklist API
  slug: mojang-blocklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-blocklist-api-openapi.yml
- filename: mojang-capes-api-openapi.yml
  format: yaml
  label: Mojang Capes API
  slug: mojang-capes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-capes-api-openapi.yml
- filename: mojang-entitlements-api-openapi.yml
  format: yaml
  label: Mojang Entitlements API
  slug: mojang-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-entitlements-api-openapi.yml
- filename: mojang-friends-api-openapi.yml
  format: yaml
  label: Mojang Friends API
  slug: mojang-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-friends-api-openapi.yml
- filename: mojang-identity-api-openapi.yml
  format: yaml
  label: Mojang Identity API
  slug: mojang-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-identity-api-openapi.yml
- filename: mojang-keys-api-openapi.yml
  format: yaml
  label: Mojang Keys API
  slug: mojang-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-keys-api-openapi.yml
- filename: mojang-presence-api-openapi.yml
  format: yaml
  label: Mojang Presence API
  slug: mojang-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-presence-api-openapi.yml
- filename: mojang-profile-api-openapi.yml
  format: yaml
  label: Mojang Profile API
  slug: mojang-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-profile-api-openapi.yml
- filename: mojang-server-api-openapi.yml
  format: yaml
  label: Mojang Server API
  slug: mojang-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-server-api-openapi.yml
- filename: mojang-session-api-openapi.yml
  format: yaml
  label: Mojang Session API
  slug: mojang-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-session-api-openapi.yml
- filename: mojang-skins-api-openapi.yml
  format: yaml
  label: Mojang Skins API
  slug: mojang-skins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-skins-api-openapi.yml
- filename: mojang-textures-api-openapi.yml
  format: yaml
  label: Mojang Textures API
  slug: mojang-textures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-textures-api-openapi.yml
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
