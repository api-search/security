---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentline-nz-api-openapi.json
  format: json
  label: Agentline API API
  slug: agentline-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-nz/openapi/_original/agentline-nz-api-openapi.json
auth_types: []
description: Agentline NZ uses a static API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentline Nz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentline NZ declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agentline NZ
provider_slug: agentline-nz
scheme_count: 1
schemes:
- evidence: Add an agentline entry under mcp.servers in OpenClaw's config with url https://agentline.nz/mcp, transport streamable-http and an Authorization header of Bearer ${AGENTLINE_KEY}
  header: Authorization
  how_to_obtain: Create a key under Dashboard → API keys in the Agentline NZ dashboard and store it in an environment variable such as AGENTLINE_KEY.
  location: header
  name: Bearer
  type: http-bearer
slug: agentline-nz-authentication
source_filename: agentline-nz-authentication.yml
source_heading: Authentication Profile
source_url: https://agentline.nz/integrations/openclaw.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentline.nz/integrations/openclaw.md\nsources:\n- https://agentline.nz/integrations/openclaw.md\n- https://agentline.nz/help/how-to-create-an-api-key.md\ndescription: Agentline NZ uses a static API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Add an agentline entry under mcp.servers in OpenClaw's config with url https://agentline.nz/mcp, transport streamable-http and an\n    Authorization header of Bearer ${AGENTLINE_KEY}\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key under Dashboard → API keys in the Agentline NZ dashboard and store it in an environment variable such as AGENTLINE_KEY.\nnote: No OAuth flows or other authentication schemes are documented on the provided pages.\ndocs: https://agentline.nz/integrations/openclaw.md\n"
source_yaml_url: https://artifacts.apis.io/agentline-nz/authentication/agentline-nz-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Email
- Assistant
- NZ
- Software-as-a-Service
- Company
---
