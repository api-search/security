---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailforbots-com-openapi-generated.yml
  format: yaml
  label: Mail for Bots API
  slug: mailforbots-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailforbots-com/openapi/_ae-authored/mailforbots-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for Mail for Bots API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mail for Bots Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mail for Bots declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mail for Bots
provider_slug: mailforbots-com
scheme_count: 1
schemes:
- evidence: API keys (they start with `bm_`) authenticate agents over REST and MCP.
  header: Authorization
  how_to_obtain: 'Keys are created by a signed-in person: in the webmail under Settings, API keys & MCP, Create key, or with POST /api/v1/keys from a webmail session.'
  location: header
  name: API key
  type: http-bearer
slug: mailforbots-com-authentication
source_filename: mailforbots-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mailforbots.com/docs/keys.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mailforbots.com/docs/keys.md\nsources:\n- https://mailforbots.com/docs/keys.md\n- https://mailforbots.com/docs/keys\n- https://mailforbots.com/blog/cursor-codex-gemini-email-mcp-setup.md\n- https://mailforbots.com/docs/quickstart.md\ndescription: Authentication schemes for Mail for Bots API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: API keys (they start with `bm_`) authenticate agents over REST and MCP.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Keys are created by a signed-in person: in the webmail under Settings, API keys & MCP, Create key, or with POST /api/v1/keys\n    from a webmail session.'\nnote: Mail for Bots does not support OAuth2, http-basic, jwt, hmac, mtls, or other authentication types.\ndocs: https://mailforbots.com/docs/keys.md\n"
source_yaml_url: https://artifacts.apis.io/mailforbots-com/authentication/mailforbots-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Artificial Intelligence
- Automation
- Software-as-a-Service
---
