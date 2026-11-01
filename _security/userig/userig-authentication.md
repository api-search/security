---
anonymous_access: false
api_key_in: []
api_specs:
- filename: userig-rig-api-api-openapi.yml
  format: yaml
  label: Rig API
  slug: rig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userig/openapi/userig-rig-api-api-openapi.yml
- filename: userig-openapi-generated.yml
  format: yaml
  label: Rig API
  slug: userig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userig/openapi/_ae-authored/userig-openapi-generated.yml
auth_types: []
description: Authentication methods documented for Rig
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Userig Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rig declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Rig
provider_slug: userig
scheme_count: 2
schemes:
- evidence: Rig runs a local MCP hub that speaks Streamable HTTP on 127.0.0.1 , port 47823 by default, and asks for a bearer token.
  header: Authorization
  how_to_obtain: 'Set on the Railway acp service; clients send Authorization: Bearer … .'
  location: header
  name: ACP_SECRET
  type: http-bearer
- evidence: You can also send X-Rig-Token on cloud requests, or type set token <rig_at_…> in an ACP chat.
  header: X-Rig-Token
  how_to_obtain: A personal developer token from Account → Security → Developer tokens. It starts with rig_at_ , is shown once at creation, and is stored hashed.
  location: header
  name: RIG_TOKEN
  type: apiKey
slug: userig-authentication
source_filename: userig-authentication.yml
source_heading: Authentication Profile
source_url: https://userig.app/learn/mcp-for-coding-agents
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://userig.app/learn/mcp-for-coding-agents\nsources:\n- https://userig.app/learn/mcp-for-coding-agents\n- https://userig.app/docs/acp-auth\n- https://userig.app/for-solo-developers\n- https://userig.app/docs/setup-diagnose\ndescription: Authentication methods documented for Rig\nschemes:\n- type: http-bearer\n  name: ACP_SECRET\n  evidence: Rig runs a local MCP hub that speaks Streamable HTTP on 127.0.0.1 , port 47823 by default, and asks for a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Set on the Railway acp service; clients send Authorization: Bearer … .'\n- type: apiKey\n  name: RIG_TOKEN\n  evidence: You can also send X-Rig-Token on cloud requests, or type set token <rig_at_…> in an ACP chat.\n  location: header\n  header: X-Rig-Token\n  how_to_obtain: A personal developer token from Account → Security → Developer tokens. It starts with\
  \ rig_at_ , is shown once at creation, and\n    is stored hashed.\ndocs: https://userig.app/learn/mcp-for-coding-agents\n"
source_yaml_url: https://artifacts.apis.io/userig/authentication/userig-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Development
- Mac
- Windows
- Process-Manager
---
