---
anonymous_access: false
api_key_in: []
auth_types: []
description: OAuth2 authentication via Google sign‑in
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MediaFast Authentication
name_suffix: Authentication
oauth_flows: []
overview: MediaFast declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MediaFast
provider_slug: mediafa-st
scheme_count: 1
schemes:
- evidence: sign in with Google and approve it
  flows:
  - authorization_code
  how_to_obtain: User clicks the Add custom connector button, enters the MediaFast MCP server URL, then a Google sign‑in popup appears; the user signs in with their Google account and clicks Approve to complete the OAuth handshake.
  name: Google OAuth
  type: oauth2
slug: mediafa-st-authentication
source_filename: mediafa-st-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mediafa.st/why-is-no-one-signing-up-for-my-saas
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mediafa.st/why-is-no-one-signing-up-for-my-saas\nsources:\n- https://www.mediafa.st/why-is-no-one-signing-up-for-my-saas\n- https://www.mediafa.st/how-to-connect-reddit-to-chatgpt\n- https://www.mediafa.st/how-to-connect-reddit-to-claude\n- https://www.mediafa.st/bluesky-scheduler\ndescription: OAuth2 authentication via Google sign‑in\nschemes:\n- type: oauth2\n  name: Google OAuth\n  evidence: sign in with Google and approve it\n  flows:\n  - authorization_code\n  how_to_obtain: User clicks the Add custom connector button, enters the MediaFast MCP server URL, then a Google sign‑in popup appears; the user\n    signs in with their Google account and clicks Approve to complete the OAuth handshake.\ndocs: https://www.mediafa.st/why-is-no-one-signing-up-for-my-saas\n"
source_yaml_url: https://artifacts.apis.io/mediafa-st/authentication/mediafa-st-authentication.yml
summary_line: 1 scheme
tags:
- Reddit
- Marketing
- Software-as-a-Service
- Community
- Automation
---
