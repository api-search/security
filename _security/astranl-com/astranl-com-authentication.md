---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for AstraNL public MCP tools and REST agent routes.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Astranl Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: astranl-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: astranl-com
provider_slug: astranl-com
scheme_count: 2
schemes:
- evidence: REST agent routes under /api/agents/ use the X-Agent-Key header with the api_key returned by POST /api/agents/register.
  header: X-Agent-Key
  how_to_obtain: Obtain the api_key by calling POST /api/agents/register.
  location: header
  name: X-Agent-Key
  type: apiKey
- evidence: The public MCP tools need no API key.
  name: none
  type: other
slug: astranl-com-authentication
source_filename: astranl-com-authentication.yml
source_heading: Authentication Profile
source_url: https://astranl.com/uk/agents/quickstart/
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://astranl.com/uk/agents/quickstart/\nsources:\n- https://astranl.com/uk/agents/quickstart/\n- https://astranl.com/nl/agents/quickstart/\n- https://astranl.com/en/agents/quickstart/\n- https://astranl.com/agents/quickstart\ndescription: Authentication methods for AstraNL public MCP tools and REST agent routes.\nschemes:\n- type: apiKey\n  name: X-Agent-Key\n  evidence: REST agent routes under /api/agents/ use the X-Agent-Key header with the api_key returned by POST /api/agents/register.\n  location: header\n  header: X-Agent-Key\n  how_to_obtain: Obtain the api_key by calling POST /api/agents/register.\n- type: other\n  name: none\n  evidence: The public MCP tools need no API key.\ndocs: https://astranl.com/uk/agents/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/astranl-com/authentication/astranl-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Coordination
- Payments
- Platform
- NL
---
