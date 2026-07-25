---
api_key_in: []
api_specs:
- filename: itch-io-auth-api-openapi.yml
  format: yaml
  label: Itch.io Auth API
  slug: itch-io-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-auth-api-openapi.yml
- filename: itch-io-builds-api-openapi.yml
  format: yaml
  label: Itch.io Builds API
  slug: itch-io-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-builds-api-openapi.yml
- filename: itch-io-bundles-api-openapi.yml
  format: yaml
  label: Itch.io Bundles API
  slug: itch-io-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-bundles-api-openapi.yml
- filename: itch-io-collections-api-openapi.yml
  format: yaml
  label: Itch.io Collections API
  slug: itch-io-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-collections-api-openapi.yml
- filename: itch-io-downloads-api-openapi.yml
  format: yaml
  label: Itch.io Downloads API
  slug: itch-io-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-downloads-api-openapi.yml
- filename: itch-io-games-api-openapi.yml
  format: yaml
  label: Itch.io Games API
  slug: itch-io-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-games-api-openapi.yml
- filename: itch-io-profile-api-openapi.yml
  format: yaml
  label: Itch.io Profile API
  slug: itch-io-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-profile-api-openapi.yml
- filename: itch-io-search-api-openapi.yml
  format: yaml
  label: Itch.io Search API
  slug: itch-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-search-api-openapi.yml
- filename: itch-io-uploads-api-openapi.yml
  format: yaml
  label: Itch.io Uploads API
  slug: itch-io-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-uploads-api-openapi.yml
- filename: itch-io-users-api-openapi.yml
  format: yaml
  label: Itch.io Users API
  slug: itch-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-users-api-openapi.yml
- filename: itch-io-wharf-api-openapi.yml
  format: yaml
  label: Itch.io Wharf API
  slug: itch-io-wharf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-wharf-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Itch Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Itch.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Itch.io
provider_slug: itch-io
scheme_count: 1
schemes:
- description: API key or JWT token issued by itch.io
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: itch-io-authentication
source_filename: itch-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key or JWT token issued by itch.io\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/authentication/itch-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Games
- Indie Games
- Game Distribution
- Game Marketplace
- Developers
---
