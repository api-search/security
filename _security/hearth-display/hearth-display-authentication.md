---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hearth Display Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hearth Display declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hearth Display
provider_slug: hearth-display
scheme_count: 2
schemes:
- evidence: Create auth.js , which fetches a fresh bearer token from the token endpoint using your client credentials.
  flows:
  - client_credentials
  how_to_obtain: Generate API credentials (client ID and client secret) in the Shopify Dev Dashboard and export them as environment variables.
  name: Shopify UCP client credentials
  token_url: https://api.shopify.com/auth/access_token
  type: oauth2
- evidence: 'How to authenticate: JWT passed with Bearer token authentication. See Authenticate your agent for a working example.'
  header: Authorization
  how_to_obtain: Fetch a bearer token at runtime from the token endpoint using client credentials.
  location: header
  name: Bearer token (JWT)
  type: http-bearer
slug: hearth-display-authentication
source_filename: hearth-display-authentication.yml
source_heading: Authentication Profile
source_url: https://shopify.dev/docs/agents/get-started/authentication
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://shopify.dev/docs/agents/get-started/authentication\nsources:\n- https://shopify.dev/docs/agents/get-started/authentication\n- https://developer.zendesk.com/documentation/authentication/\n- https://shopify.dev/docs/api/storefront/latest\n- https://shopify.dev/docs/agents/profiles/auth-and-rate-limiting\ndescription: Authentication\nschemes:\n- type: oauth2\n  name: Shopify UCP client credentials\n  evidence: Create auth.js , which fetches a fresh bearer token from the token endpoint using your client credentials.\n  flows:\n  - client_credentials\n  token_url: https://api.shopify.com/auth/access_token\n  how_to_obtain: Generate API credentials (client ID and client secret) in the Shopify Dev Dashboard and export them as environment variables.\n- type: http-bearer\n  name: Bearer token (JWT)\n  evidence: 'How to authenticate: JWT passed with Bearer token authentication. See\
  \ Authenticate your agent for a working example.'\n  location: header\n  header: Authorization\n  how_to_obtain: Fetch a bearer token at runtime from the token endpoint using client credentials.\ndocs: https://shopify.dev/docs/agents/get-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/hearth-display/authentication/hearth-display-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
