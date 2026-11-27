---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Epovest
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Epovest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epovest declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Epovest
provider_slug: epovest-com
scheme_count: 2
schemes:
- evidence: 'Use the same address with an API key in the header of every call:


    Authorization: Bearer epo_...'
  header: Authorization
  how_to_obtain: The person creates the key in the app at https://app.epovest.com/account/api-keys.
  location: header
  name: API Key
  type: http-bearer
- evidence: 'The one-click path is OAuth 2.1, authorization code with PKCE, and the client registers itself: discovery starts from the unauthenticated response of https://mcp.epovest.com/mcp, the person signs in to Epovest and approves the access, once.'
  how_to_obtain: The client registers itself via discovery from https://mcp.epovest.com/mcp and the user signs in and approves access.
  name: OAuth 2.1 Authorization Code with PKCE
  type: oauth2
slug: epovest-com-authentication
source_filename: epovest-com-authentication.yml
source_heading: Authentication Profile
source_url: https://epovest.com/docs/setup.md
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://epovest.com/docs/setup.md\nsources:\n- https://epovest.com/docs/setup.md\ndescription: Authentication methods for Epovest\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Use the same address with an API key in the header of every call:\n\n\n    Authorization: Bearer epo_...'\n  location: header\n  header: Authorization\n  how_to_obtain: The person creates the key in the app at https://app.epovest.com/account/api-keys.\n- type: oauth2\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: 'The one-click path is OAuth 2.1, authorization code with PKCE, and the client registers itself: discovery starts from the unauthenticated\n    response of https://mcp.epovest.com/mcp, the person signs in to Epovest and approves the access, once.'\n  how_to_obtain: The client registers itself via discovery from https://mcp.epovest.com/mcp and the user signs in and approves\
  \ access.\ndocs: https://epovest.com/docs/setup.md\n"
source_yaml_url: https://artifacts.apis.io/epovest-com/authentication/epovest-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Reputation
- Platform
- Analytics
- Company
---
