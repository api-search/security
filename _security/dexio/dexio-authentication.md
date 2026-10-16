---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dexio-openapi-generated.yml
  format: yaml
  label: Dexio API
  slug: dexio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexio/refs/heads/main/openapi/_ae-authored/dexio-openapi-generated.yml
auth_types: []
description: Dexio authentication uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dexio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dexio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dexio
provider_slug: dexio
scheme_count: 1
schemes:
- evidence: http_headers = { "Authorization" = "Bearer dxk_..." }
  header: Authorization
  how_to_obtain: Obtain the API key (dxk_…) by sending a Dexio setup message to the agent, which returns a link and code; after signing in and allowing access, Dexio provides the API key.
  location: header
  name: Authorization
  type: http-bearer
slug: dexio-authentication
source_filename: dexio-authentication.yml
source_heading: Authentication Profile
source_url: https://dexio.wiki/guides/codex-mcp/
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dexio.wiki/guides/codex-mcp/\nsources:\n- https://dexio.wiki/guides/codex-mcp/\n- https://dexio.wiki/guides/cursor-mcp/\n- https://dexio.wiki/guides/hermes-agent-setup/\n- https://dexio.wiki/guides/openclaw-setup/\ndescription: Dexio authentication uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: http_headers = { \"Authorization\" = \"Bearer dxk_...\" }\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the API key (dxk_…) by sending a Dexio setup message to the agent, which returns a link and code; after signing in and\n    allowing access, Dexio provides the API key.\nnote: No OAuth2, API key, or other authentication methods are documented on the provided pages.\ndocs: https://dexio.wiki/guides/codex-mcp/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexio/refs/heads/main/authentication/dexio-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Wiki
- Knowledge-Management
- Agent-Integration
- Open-Source
---
