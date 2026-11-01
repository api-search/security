---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Skybridge
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Skybridge Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: skybridge-tech declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: skybridge-tech
provider_slug: skybridge-tech
scheme_count: 1
schemes:
- authorize_url: https://auth.myshop.com/authorize
  evidence: 'Once the user is signed in, every request carries Authorization: Bearer <token> .'
  header: Authorization
  how_to_obtain: Obtain a token from the configured OAuth provider (e.g., Auth0, Clerk, Descope, Stytch, WorkOS) using the standard OAuth 2.0 authorization code flow.
  location: header
  name: OAuth2
  scopes:
  - checkout
  - shop.read
  token_url: https://auth.myshop.com/token
  type: oauth2
slug: skybridge-tech-authentication
source_filename: skybridge-tech-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.skybridge.tech/build/auth
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.skybridge.tech/build/auth\nsources:\n- https://docs.skybridge.tech/build/auth\n- https://docs.skybridge.tech/api-reference/mcp-auth-metadata-router\n- https://docs.skybridge.tech/api-reference/optional-bearer-auth\n- https://docs.skybridge.tech/api-reference/require-bearer-auth\ndescription: Authentication schemes for Skybridge\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: 'Once the user is signed in, every request carries Authorization: Bearer <token> .'\n  location: header\n  header: Authorization\n  token_url: https://auth.myshop.com/token\n  authorize_url: https://auth.myshop.com/authorize\n  scopes:\n  - checkout\n  - shop.read\n  how_to_obtain: Obtain a token from the configured OAuth provider (e.g., Auth0, Clerk, Descope, Stytch, WorkOS) using the standard OAuth 2.0\n    authorization code flow.\ndocs: https://docs.skybridge.tech/build/auth\n"
source_yaml_url: https://artifacts.apis.io/skybridge-tech/authentication/skybridge-tech-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Framework
- OpenSource
- TypeScript
- AI
---
