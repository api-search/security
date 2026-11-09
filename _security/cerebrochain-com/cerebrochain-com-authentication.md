---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published by CerebroChain
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cerebrochain Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CerebroChain declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CerebroChain
provider_slug: cerebrochain-com
scheme_count: 2
schemes:
- authorize_url: https://cerebrochain.com/api/oauth/authorize
  evidence: Give your app or agent scoped, per-user access to CerebroChain's metered bot API through a standard OAuth 2.1 authorization-code + PKCE flow — consent screen, granular scopes, refresh-token rotation, and revocation.
  flows:
  - authorization_code
  how_to_obtain: Register an OAuth app in the console (Settings → OAuth apps) to receive a client_id and, for confidential apps, a client_secret.
  name: OAuth 2.1 Authorization Code with PKCE
  scopes:
  - bot:read
  - bot:invoke
  - credits:read
  - keys:manage
  - wms:read
  - logistics:read
  - executive:read
  - wms:write
  - logistics:write
  - discovery
  - mcp
  type: oauth2
- evidence: API key (machine-to-machine). For your own backend agents, issue a key in the console and send it as the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Issue a key in the CerebroChain console under Settings → API keys.
  location: header
  name: API Key
  type: apiKey
slug: cerebrochain-com-authentication
source_filename: cerebrochain-com-authentication.yml
source_heading: Authentication Profile
source_url: https://cerebrochain.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cerebrochain.com/.well-known/oauth-authorization-server\nsources:\n- https://cerebrochain.com/.well-known/oauth-authorization-server\n- https://cerebrochain.com/developers\n- https://cerebrochain.com/connect\ndescription: Authentication methods published by CerebroChain\nschemes:\n- type: oauth2\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: Give your app or agent scoped, per-user access to CerebroChain's metered bot API through a standard OAuth 2.1 authorization-code +\n    PKCE flow — consent screen, granular scopes, refresh-token rotation, and revocation.\n  flows:\n  - authorization_code\n  authorize_url: https://cerebrochain.com/api/oauth/authorize\n  scopes:\n  - bot:read\n  - bot:invoke\n  - credits:read\n  - keys:manage\n  - wms:read\n  - logistics:read\n  - executive:read\n  - wms:write\n  - logistics:write\n  - discovery\n  - mcp\n  how_to_obtain:\
  \ Register an OAuth app in the console (Settings → OAuth apps) to receive a client_id and, for confidential apps, a client_secret.\n- type: apiKey\n  name: API Key\n  evidence: API key (machine-to-machine). For your own backend agents, issue a key in the console and send it as the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Issue a key in the CerebroChain console under Settings → API keys.\ndocs: https://cerebrochain.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/cerebrochain-com/authentication/cerebrochain-com-authentication.yml
summary_line: 2 schemes
tags:
- Warehouse
- Logistics
- Artificial Intelligence
- Software-as-a-Service
- Warehouse Management
---
