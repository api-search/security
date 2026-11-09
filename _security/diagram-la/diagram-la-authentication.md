---
anonymous_access: false
api_key_in: []
api_specs:
- filename: diagram-la-diagrams-api-openapi.yml
  format: yaml
  label: Diagram Diagrams API
  slug: diagram-la-diagrams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/diagram-la/openapi/diagram-la-diagrams-api-openapi.yml
- filename: diagram-la-projects-api-openapi.yml
  format: yaml
  label: Diagram Projects API
  slug: diagram-la-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/diagram-la/openapi/diagram-la-projects-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Diagram La Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diagram secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Diagram
provider_slug: diagram-la
scheme_count: 3
schemes:
- applies_to: HTTP API (https://diagram.la/api/v1) and the MCP server (https://diagram.la/mcp)
  description: Diagram API key (dgm_...)
  docs_text: 'Auth: `Authorization: Bearer dgm_...` with a key from the [API keys](https://diagram.la/keys) page.'
  key_management: API keys are stored as SHA-256 hashes, shown once, and can be revoked on the API keys page. Each key acts as the account that created it. 20 active API keys per account.
  name: bearer
  scheme: bearer
  sources:
  - openapi/diagram-la-openapi.yml
  - https://diagram.la/docs/api
  - https://diagram.la/docs/security
  type: http
- applies_to: https://diagram.la/mcp
  description: MCP sign-in for the remote MCP server only (not declared in the OpenAPI). "Sign-in follows the MCP authorization spec - OAuth 2.1 with PKCE and dynamic client registration, discovered from https://diagram.la/.well-known/oauth-protected-resource/mcp."
  discovery: https://diagram.la/.well-known/oauth-protected-resource/mcp
  dynamic_client_registration: true
  flows:
  - authorizationCode
  name: mcp-oauth
  pkce: true
  scopes_documented: false
  sources:
  - https://diagram.la/docs/chat-apps
  type: oauth2
- description: For tools that only take a URL and cannot sign in, the key is embedded in the address https://diagram.la/mcp/<your key>; the docs say to treat it like a password.
  in: path
  name: mcp-key-in-url
  sources:
  - https://diagram.la/docs/chat-apps
  type: apiKey
slug: diagram-la-authentication
source_filename: diagram-la-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://diagram.la/docs/api\ndocs: https://diagram.la/docs/api\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Diagram API key (dgm_...)\n  applies_to: HTTP API (https://diagram.la/api/v1) and the MCP server (https://diagram.la/mcp)\n  docs_text: \"Auth: `Authorization: Bearer dgm_...` with a key from the [API keys](https://diagram.la/keys) page.\"\n  key_management: API keys are stored as SHA-256 hashes, shown once, and can be revoked on the API keys page. Each key acts as the account that created it. 20 active API keys per account.\n  sources:\n  - openapi/diagram-la-openapi.yml\n  - https://diagram.la/docs/api\n  - https://diagram.la/docs/security\n- name: mcp-oauth\n  type: oauth2\n  description: MCP sign-in for the remote MCP server only (not declared in the OpenAPI). \"Sign-in follows the MCP authorization spec - OAuth 2.1 with PKCE and dynamic client\
  \ registration, discovered from https://diagram.la/.well-known/oauth-protected-resource/mcp.\"\n  applies_to: https://diagram.la/mcp\n  flows: [authorizationCode]\n  pkce: true\n  dynamic_client_registration: true\n  discovery: https://diagram.la/.well-known/oauth-protected-resource/mcp\n  scopes_documented: false\n  sources:\n  - https://diagram.la/docs/chat-apps\n- name: mcp-key-in-url\n  type: apiKey\n  in: path\n  description: For tools that only take a URL and cannot sign in, the key is embedded in the address https://diagram.la/mcp/<your key>; the docs say to treat it like a password.\n  sources:\n  - https://diagram.la/docs/chat-apps\nend_user_signin: Google or a one-time emailed link (Firebase email link); session is an httpOnly cookie (website only).\n"
source_yaml_url: https://artifacts.apis.io/diagram-la/authentication/diagram-la-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Diagramming
- Visualization
- Artificial Intelligence
- MCP
- Collaboration
- Developer Tools
---
