---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: TripLedger Authentication
name_suffix: Authentication
oauth_flows: []
overview: TripLedger declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TripLedger
provider_slug: tripledger-app
scheme_count: 2
schemes:
- evidence: 'Use a key for Claude Code or any client that sends Authorization: Bearer tl_... .'
  header: Authorization
  how_to_obtain: Create keys at Settings → API keys.
  location: header
  name: API Key
  type: http-bearer
- authorize_url: https://my.tripledger.app/api/auth/oauth2/authorize
  evidence: TripLedger supports agent access to a user's private travel ledger through OAuth 2.1 Authorization Code with PKCE and explicit human approval.
  header: Authorization
  how_to_obtain: Register a client via Dynamic Client Registration or provide a Client ID Metadata Document, then follow the Authorization Code with PKCE flow.
  location: header
  name: TripLedger MCP OAuth
  scopes:
  - ledger:read
  - ledger:write
  type: oauth2
slug: tripledger-app-authentication
source_filename: tripledger-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tripledger.app/connect/credentials/
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tripledger.app/connect/credentials/\nsources:\n- https://docs.tripledger.app/connect/credentials/\n- https://my.tripledger.app/auth.md\n- https://docs.tripledger.app/introduction/getting-started/\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Use a key for Claude Code or any client that sends Authorization: Bearer tl_... .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys at Settings → API keys.\n- type: oauth2\n  name: TripLedger MCP OAuth\n  evidence: TripLedger supports agent access to a user's private travel ledger through OAuth 2.1 Authorization Code with PKCE and explicit human\n    approval.\n  location: header\n  header: Authorization\n  authorize_url: https://my.tripledger.app/api/auth/oauth2/authorize\n  scopes:\n  - ledger:read\n  - ledger:write\n  how_to_obtain: Register a client via Dynamic Client Registration or\
  \ provide a Client ID Metadata Document, then follow the Authorization Code\n    with PKCE flow.\ndocs: https://docs.tripledger.app/connect/credentials/\n"
source_yaml_url: https://artifacts.apis.io/tripledger-app/authentication/tripledger-app-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Travel
- TaxResidency
- AI
- Schengen
---
