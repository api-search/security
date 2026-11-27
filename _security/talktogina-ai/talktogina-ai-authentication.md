---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Talk To Gina agents
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Talk To Gina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talk To Gina declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Talk To Gina
provider_slug: talktogina-ai
scheme_count: 2
schemes:
- evidence: It takes a key in the Authorization header, as Bearer <key>.
  header: Authorization
  how_to_obtain: Create a key on the Access page in the console; copy the shown key and use it as the Bearer token in the Authorization header.
  location: header
  name: Bearer token
  type: apiKey
- evidence: Press Create app client and copy the Client ID , the Client secret (shown once), the Authorization URL , the Token URL (also the refresh URL) and the Scopes into the app.
  how_to_obtain: Create an app client on the Access page under App clients; copy the Client ID, Client secret, Authorization URL, Token URL, and Scopes.
  name: App client
  type: oauth2
slug: talktogina-ai-authentication
source_filename: talktogina-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://app.talktogina.ai/docs/agent-api-keys
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.talktogina.ai/docs/agent-api-keys\nsources:\n- https://app.talktogina.ai/docs/agent-api-keys\n- https://app.talktogina.ai/docs/security\n- https://app.talktogina.ai/docs/credentials\n- https://app.talktogina.ai/docs/getting-started\ndescription: Authentication methods for Talk To Gina agents\nschemes:\n- type: apiKey\n  name: Bearer token\n  evidence: It takes a key in the Authorization header, as Bearer <key>.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key on the Access page in the console; copy the shown key and use it as the Bearer token in the Authorization header.\n- type: oauth2\n  name: App client\n  evidence: Press Create app client and copy the Client ID , the Client secret (shown once), the Authorization URL , the Token URL (also the refresh\n    URL) and the Scopes into the app.\n  how_to_obtain: Create an app client on the Access\
  \ page under App clients; copy the Client ID, Client secret, Authorization URL, Token URL, and\n    Scopes.\ndocs: https://app.talktogina.ai/docs/agent-api-keys\n"
source_yaml_url: https://artifacts.apis.io/talktogina-ai/authentication/talktogina-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Automation
- Business
- Productivity
- SaaS
---
