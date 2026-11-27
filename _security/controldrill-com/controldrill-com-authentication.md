---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ControlDrill Authentication
name_suffix: Authentication
oauth_flows: []
overview: ControlDrill declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ControlDrill
provider_slug: controldrill-com
scheme_count: 1
schemes:
- applies_to: https://mcp.controldrill.com/mcp
  description: 'MCP server auth: "OAuth 2.1 via WorkOS AuthKit (no API keys)". The client discovers OAuth from the server metadata and opens a browser login.'
  name: oauth2
  provider: WorkOS AuthKit
  type: oauth2
slug: controldrill-com-authentication
source_filename: controldrill-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://github.com/controldrill/mcp\ndocs: https://github.com/controldrill/mcp\nschemes:\n- name: oauth2\n  type: oauth2\n  applies_to: https://mcp.controldrill.com/mcp\n  description: 'MCP server auth: \"OAuth 2.1 via WorkOS AuthKit (no API keys)\". The client discovers OAuth from the server metadata and opens a browser login.'\n  provider: WorkOS AuthKit\napi_keys: false\nnote: There is no REST API or OpenAPI. The only documented programmatic surface is the remote MCP server, and a paid plan is required to use it.\n"
source_yaml_url: https://artifacts.apis.io/controldrill-com/authentication/controldrill-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Incident Response
- Tabletop Exercises
- Compliance
- Security
- SOC 2
- Audit Evidence
- MCP
---
