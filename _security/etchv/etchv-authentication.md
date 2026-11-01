---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Etchv Authentication
name_suffix: Authentication
oauth_flows: []
overview: etchv declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: etchv
provider_slug: etchv
scheme_count: 1
schemes:
- evidence: Send your API key in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Create a key in the Etchv dashboard, copy the secret, and keep it on your server.
  location: header
  name: X-API-Key
  scopes:
  - watermarks:embed
  - watermarks:detect
  - assets:read
  - assets:write
  - assets:delete
  - webhooks:read
  - webhooks:write
  - storage:read
  - storage:write
  type: apiKey
slug: etchv-authentication
source_filename: etchv-authentication.yml
source_heading: Authentication Profile
source_url: https://etchv.com/docs/authentication
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://etchv.com/docs/authentication\nsources:\n- https://etchv.com/docs/authentication\n- https://etchv.com/docs/quickstart\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Send your API key in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  scopes:\n  - watermarks:embed\n  - watermarks:detect\n  - assets:read\n  - assets:write\n  - assets:delete\n  - webhooks:read\n  - webhooks:write\n  - storage:read\n  - storage:write\n  how_to_obtain: Create a key in the Etchv dashboard, copy the secret, and keep it on your server.\ndocs: https://etchv.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/etchv/authentication/etchv-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Watermarking
- Media
- Security
- Developer Tools
---
