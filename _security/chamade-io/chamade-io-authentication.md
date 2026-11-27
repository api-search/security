---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Chamade
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chamade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chamade declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chamade
provider_slug: chamade-io
scheme_count: 2
schemes:
- evidence: 'Auth is either a standard Authorization: Bearer chmd_* header (same API key as the REST API, best for config-file clients) or the MCP OAuth 2.1 flow with Dynamic Client Registration (used by claude.ai Custom Connectors — paste the URL, sign in, done).'
  header: Authorization
  how_to_obtain: Mint an agent key on the dashboard (starts with chmd_) and place it after "Bearer " in the Authorization header.
  location: header
  name: Bearer token
  type: http-bearer
- authorize_url: https://mcp.chamade.io/mcp-auth/consent
  evidence: Chamade runs an OAuth 2.1 authorization server (Dynamic Client Registration + PKCE) so the client registers itself on the fly, the user approves once in a consent screen at chamade.io/mcp-auth/consent, and an opaque access token is issued.
  flows:
  - authorizationCode
  header: Authorization
  how_to_obtain: Client initiates OAuth 2.1 flow with Dynamic Client Registration; user consents at the consent screen and receives an access token.
  location: header
  name: MCP OAuth 2.1
  type: oauth2
slug: chamade-io-authentication
source_filename: chamade-io-authentication.yml
source_heading: Authentication Profile
source_url: https://chamade.io/llms-setup.txt
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://chamade.io/llms-setup.txt\nsources:\n- https://chamade.io/llms-setup.txt\n- https://chamade.io/docs/quickstart\n- https://chamade.io/docs/mcp\n- https://chamade.io/docs/voice-providers\ndescription: Authentication methods for Chamade\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Auth is either a standard Authorization: Bearer chmd_* header (same API key as the REST API, best for config-file clients) or the\n    MCP OAuth 2.1 flow with Dynamic Client Registration (used by claude.ai Custom Connectors — paste the URL, sign in, done).'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint an agent key on the dashboard (starts with chmd_) and place it after \"Bearer \" in the Authorization header.\n- type: oauth2\n  name: MCP OAuth 2.1\n  evidence: Chamade runs an OAuth 2.1 authorization server (Dynamic Client Registration + PKCE) so the client\
  \ registers itself on the fly, the\n    user approves once in a consent screen at chamade.io/mcp-auth/consent, and an opaque access token is issued.\n  location: header\n  header: Authorization\n  flows:\n  - authorizationCode\n  authorize_url: https://mcp.chamade.io/mcp-auth/consent\n  how_to_obtain: Client initiates OAuth 2.1 flow with Dynamic Client Registration; user consents at the consent screen and receives an access\n    token.\ndocs: https://chamade.io/llms-setup.txt\n"
source_yaml_url: https://artifacts.apis.io/chamade-io/authentication/chamade-io-authentication.yml
summary_line: 2 schemes
tags:
- Voice gateway
- Chat gateway
- AI Agents
- SIP
- Speech API
---
