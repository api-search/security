---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dibatto-com-episodes-api-openapi.yml
  format: yaml
  label: Dibatto Episodes API
  slug: dibatto-com-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dibatto-com/openapi/dibatto-com-episodes-api-openapi.yml
- filename: dibatto-com-shows-api-openapi.yml
  format: yaml
  label: Dibatto Shows API
  slug: dibatto-com-shows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dibatto-com/openapi/dibatto-com-shows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dibatto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dibatto secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dibatto
provider_slug: dibatto-com
scheme_count: 1
schemes:
- description: Create a scoped, expiring API key under Plan and credits → API connections in Dibatto. Studio required.
  in: header
  key_lifecycle:
    creation: In Plan and credits → API connections, name the connection, choose its permissions and an expiry of 7, 30 or 90 days, then create a key.
    expiry_options_days:
    - 7
    - 30
    - 90
    plan_required: Studio
    retrievable_after_creation: false
    revocation: Revoke a key in Dibatto to disconnect the tool immediately.
  name: apiKey
  parameter: x-api-key
  permission_declaration: Each operation declares its required permission in the vendor extension x-required-scope.
  permissions:
  - description: read owned shows, rundowns, the episode library, episode desks, transcripts and wrap progress.
    name: studio:read
  - description: generate a rundown using an existing show's beat, co-host and sources.
    name: rundown:prepare
  - description: create a private draft using an owned show and, optionally, its rundown.
    name: episode:prepare
  sources:
  - openapi/dibatto-com-openapi.yml
  - https://dibatto.com/developers
  type: apiKey
slug: dibatto-com-authentication
source_filename: dibatto-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dibatto.com/developers\ndocs: https://dibatto.com/developers\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Create a scoped, expiring API key under Plan and credits → API connections in\n    Dibatto. Studio required.\n  sources:\n  - openapi/dibatto-com-openapi.yml\n  - https://dibatto.com/developers\n  key_lifecycle:\n    creation: \"In Plan and credits → API connections, name the connection, choose its permissions and an expiry of 7, 30 or 90 days, then create a key.\"\n    expiry_options_days: [7, 30, 90]\n    retrievable_after_creation: false\n    revocation: \"Revoke a key in Dibatto to disconnect the tool immediately.\"\n    plan_required: Studio\n  permissions:\n  - name: studio:read\n    description: read owned shows, rundowns, the episode library, episode desks, transcripts and wrap progress.\n  - name:\
  \ rundown:prepare\n    description: generate a rundown using an existing show's beat, co-host and sources.\n  - name: episode:prepare\n    description: create a private draft using an owned show and, optionally, its rundown.\n  permission_declaration: Each operation declares its required permission in the vendor extension x-required-scope.\nnote: Permissions are API-key permissions, not OAuth scopes; the API documents no OAuth flow.\n"
source_yaml_url: https://artifacts.apis.io/dibatto-com/authentication/dibatto-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Podcasts
- Artificial Intelligence
- Voice
- Audio
- Content Creation
- MCP
---
