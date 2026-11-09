---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Two credential types work interchangeably at https://api.agently.dev/mcp, both sent as a standard bearer token:'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agently Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agently declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Agently
provider_slug: agently-dev
scheme_count: 2
schemes:
- evidence: API keys ( agently_sk_... )
  header: Authorization
  how_to_obtain: Minted in the app under Settings → API keys (or Brain → Connect an agent) by any workspace member.
  location: header
  name: API key
  type: http-bearer
- authorize_url: https://api.agently.dev/oauth/authorize
  evidence: OAuth 2.1 ( agently_at_... )
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Client registration via POST https://api.agently.dev/oauth/register returns a client_id; then use the authorization endpoint to obtain a code and exchange it at https://api.agently.dev/oauth/token.
  location: header
  name: OAuth 2.1
  scopes:
  - brain:read
  - brain:write
  type: oauth2
slug: agently-dev-authentication
source_filename: agently-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://agently.dev/docs/mcp-authentication
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agently.dev/docs/mcp-authentication\nsources:\n- https://agently.dev/docs/mcp-authentication\n- https://agently.dev/help/credits-and-your-own-api-key\n- https://agently.dev/docs/getting-started\n- https://agently.dev/help/getting-started-on-the-web\ndescription: 'Two credential types work interchangeably at https://api.agently.dev/mcp, both sent as a standard bearer token:'\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: API keys ( agently_sk_... )\n  location: header\n  header: Authorization\n  how_to_obtain: Minted in the app under Settings → API keys (or Brain → Connect an agent) by any workspace member.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: OAuth 2.1 ( agently_at_... )\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://api.agently.dev/oauth/authorize\n  scopes:\n  - brain:read\n  - brain:write\n\
  \  how_to_obtain: Client registration via POST https://api.agently.dev/oauth/register returns a client_id; then use the authorization endpoint\n    to obtain a code and exchange it at https://api.agently.dev/oauth/token.\ndocs: https://agently.dev/docs/mcp-authentication\n"
source_yaml_url: https://artifacts.apis.io/agently-dev/authentication/agently-dev-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Automation
- Productivity
- Software-as-a-Service
- Chief of Staff
---
