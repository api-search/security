---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for BotPhone as described on the documentation page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Botphone Tel Authentication
name_suffix: Authentication
oauth_flows: []
overview: BotPhone declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BotPhone
provider_slug: botphone-tel
scheme_count: 2
schemes:
- evidence: Use the server URL above with OAuth 2.0 (authorization code with PKCE, dynamic client registration).
  flows:
  - authorization_code
  how_to_obtain: Dynamic client registration via the discovery endpoint at https://auth.botphone.tel/.well-known/oauth-protected-resource.
  name: BotPhone OAuth
  type: oauth2
- evidence: 'If your client takes an API key instead, create one in the dashboard under Connect your AI assistant and send it as Authorization: Bearer <key> or X-API-Key: <key>.'
  header: Authorization
  how_to_obtain: Create an API key in the BotPhone dashboard under Connect your AI assistant.
  location: header
  name: BotPhone API key
  type: apiKey
slug: botphone-tel-authentication
source_filename: botphone-tel-authentication.yml
source_heading: Authentication Profile
source_url: https://auth.botphone.tel/docs
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://auth.botphone.tel/docs\nsources:\n- https://auth.botphone.tel/docs\ndescription: Authentication methods for BotPhone as described on the documentation page.\nschemes:\n- type: oauth2\n  name: BotPhone OAuth\n  evidence: Use the server URL above with OAuth 2.0 (authorization code with PKCE, dynamic client registration).\n  flows:\n  - authorization_code\n  how_to_obtain: Dynamic client registration via the discovery endpoint at https://auth.botphone.tel/.well-known/oauth-protected-resource.\n- type: apiKey\n  name: BotPhone API key\n  evidence: 'If your client takes an API key instead, create one in the dashboard under Connect your AI assistant and send it as Authorization:\n    Bearer <key> or X-API-Key: <key>.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the BotPhone dashboard under Connect your AI assistant.\ndocs: https://auth.botphone.tel/docs\n"
source_yaml_url: https://artifacts.apis.io/botphone-tel/authentication/botphone-tel-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Telephony
- Receptionist
- Software-as-a-Service
- BotPhone
---
