---
anonymous_access: false
api_key_in: []
api_specs:
- filename: letl-ink-openapi-generated.yml
  format: yaml
  label: Letlink API
  slug: letl-ink-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letl-ink/openapi/_ae-authored/letl-ink-openapi-generated.yml
auth_types: []
description: Authentication for Letlink REST API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Letlink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Letlink declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Letlink
provider_slug: letl-ink
scheme_count: 2
schemes:
- evidence: 'Send the token as X-API-KEY or as Authorization: Bearer . Both are accepted on /api/v1 and on /mcp .'
  header: X-API-KEY
  how_to_obtain: Generate a token in the workspace Integrations → REST API page; the token does not expire.
  location: header
  name: X-API-KEY
  type: apiKey
- evidence: 'Send the token as X-API-KEY or as Authorization: Bearer . Both are accepted on /api/v1 and on /mcp .'
  header: Authorization
  how_to_obtain: Generate a token in the workspace Integrations → REST API page; the token does not expire.
  location: header
  name: Authorization
  type: http-bearer
slug: letl-ink-authentication
source_filename: letl-ink-authentication.yml
source_heading: Authentication Profile
source_url: https://letl.ink/help-center/two-factor-authentication
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://letl.ink/help-center/two-factor-authentication\nsources:\n- https://letl.ink/help-center/two-factor-authentication\n- https://letl.ink/help-center/rest-api#auth-me\ndescription: Authentication for Letlink REST API\nschemes:\n- type: apiKey\n  name: X-API-KEY\n  evidence: 'Send the token as X-API-KEY or as Authorization: Bearer . Both are accepted on /api/v1 and on /mcp .'\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Generate a token in the workspace Integrations → REST API page; the token does not expire.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Send the token as X-API-KEY or as Authorization: Bearer . Both are accepted on /api/v1 and on /mcp .'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a token in the workspace Integrations → REST API page; the token does not expire.\ndocs: https://letl.ink/help-center/two-factor-authentication\n"
source_yaml_url: https://artifacts.apis.io/letl-ink/authentication/letl-ink-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Link Shortener
- Analytics
- Custom Domains
- QR Codes
---
