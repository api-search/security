---
anonymous_access: false
api_key_in: []
api_specs:
- filename: synci-io-openapi-generated.yml
  format: yaml
  label: Synci API
  slug: synci-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synci-io/openapi/_ae-authored/synci-io-openapi-generated.yml
auth_types: []
description: Synci API authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Synci Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synci declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Synci
provider_slug: synci-io
scheme_count: 2
schemes:
- evidence: 'Every API request is authenticated with a Bearer token in the `Authorization` header:'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- authorize_url: https://api.synci.io/oauth/authorize
  evidence: Synci implements **OAuth 2.0 authorization code grant with PKCE**.
  header: Authorization
  how_to_obtain: Create a token in the Synci dashboard under Developers → API tokens for personal access tokens, or register an OAuth app under Developers → Apps and follow the authorization code flow with PKCE to obtain an access token.
  location: header
  name: OAuth 2.0 authorization code grant with PKCE
  scopes:
  - profile:read
  - accounts:read
  - accounts:write
  - transactions:read
  - transactions:write
  - sensitive:read
  - financial-connections:read
  - financial-connections:write
  - transfer-links:read
  - transfer-links:write
  - rules:read
  - rules:write
  - webhooks:read
  - webhooks:write
  - destinations:read
  - destinations:write
  token_url: https://api.synci.io/oauth/token
  type: oauth2
slug: synci-io-authentication
source_filename: synci-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.synci.io/guides/authentication.md
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.synci.io/guides/authentication.md\nsources:\n- https://docs.synci.io/guides/authentication.md\n- https://docs.synci.io/guides/oauth.md\n- https://docs.synci.io/api-reference/simplefin/regenerate-setup-token.md\n- https://docs.synci.io/api-reference/simplefin/revoke-access-credentials.md\ndescription: Synci API authentication\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Every API request is authenticated with a Bearer token in the `Authorization` header:'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth 2.0 authorization code grant with PKCE\n  evidence: Synci implements **OAuth 2.0 authorization code grant with PKCE**.\n  location: header\n  header: Authorization\n  token_url: https://api.synci.io/oauth/token\n  authorize_url: https://api.synci.io/oauth/authorize\n  scopes:\n  - profile:read\n  - accounts:read\n  - accounts:write\n\
  \  - transactions:read\n  - transactions:write\n  - sensitive:read\n  - financial-connections:read\n  - financial-connections:write\n  - transfer-links:read\n  - transfer-links:write\n  - rules:read\n  - rules:write\n  - webhooks:read\n  - webhooks:write\n  - destinations:read\n  - destinations:write\n  how_to_obtain: Create a token in the Synci dashboard under Developers → API tokens for personal access tokens, or register an OAuth app under\n    Developers → Apps and follow the authorization code flow with PKCE to obtain an access token.\ndocs: https://docs.synci.io/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/synci-io/authentication/synci-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Banking
- AI
- Finance
- Integration
---
