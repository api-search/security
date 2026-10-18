---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for FlashAlpha as described on the page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Flashalpha Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flashalpha declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Flashalpha
provider_slug: flashalpha
scheme_count: 2
schemes:
- evidence: OAuth authorizes your FlashAlpha account without requiring an API key pasted into the chat.
  how_to_obtain: Standard OAuth flow via browser handoff; no client ID or secret required for the standard setup.
  name: OAuth
  type: oauth2
- evidence: FlashAlpha also exposes https://lab.flashalpha.com/mcp , whose tools accept an apiKey parameter.
  how_to_obtain: Obtain an API key from the FlashAlpha account page and include it as the "apiKey" query parameter.
  location: query
  name: apiKey
  type: apiKey
slug: flashalpha-authentication
source_filename: flashalpha-authentication.yml
source_heading: Authentication Profile
source_url: https://flashalpha.com/articles/connect-claude-to-flashalpha-mcp-oauth
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://flashalpha.com/articles/connect-claude-to-flashalpha-mcp-oauth\nsources:\n- https://flashalpha.com/articles/connect-claude-to-flashalpha-mcp-oauth\ndescription: Authentication methods for FlashAlpha as described on the page.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: OAuth authorizes your FlashAlpha account without requiring an API key pasted into the chat.\n  how_to_obtain: Standard OAuth flow via browser handoff; no client ID or secret required for the standard setup.\n- type: apiKey\n  name: apiKey\n  evidence: FlashAlpha also exposes https://lab.flashalpha.com/mcp , whose tools accept an apiKey parameter.\n  location: query\n  how_to_obtain: Obtain an API key from the FlashAlpha account page and include it as the \"apiKey\" query parameter.\ndocs: https://flashalpha.com/articles/connect-claude-to-flashalpha-mcp-oauth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flashalpha/refs/heads/main/authentication/flashalpha-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Options
- Analytics
---
