---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agnic-ai-api-reference-openapi-generated.yml
  format: yaml
  label: Agnic API Reference API
  slug: api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agnic-ai/openapi/_ae-authored/agnic-ai-api-reference-openapi-generated.yml
- filename: agnic-ai-core-openapi-generated.yml
  format: yaml
  label: Agnic core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agnic-ai/openapi/_ae-authored/agnic-ai-core-openapi-generated.yml
- filename: agnic-ai-x402-openapi-generated.yml
  format: yaml
  label: Agnic X402 API
  slug: x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agnic-ai/openapi/_ae-authored/agnic-ai-x402-openapi-generated.yml
auth_types: []
description: Authentication methods for Agnic APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agnic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agnic declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Agnic
provider_slug: agnic-ai
scheme_count: 2
schemes:
- evidence: 'Include the token in the `X-Agnic-Token` header:'
  header: X-Agnic-Token
  how_to_obtain: Generate token via Agnic Dashboard → Connect App → Generate Token (see "Creating a Token" section).
  location: header
  name: API Token
  type: apiKey
- authorize_url: https://api.agnic.ai/oauth/authorize
  evidence: Redirect users to our authorization endpoint. Include PKCE for any non-confidential client.
  how_to_obtain: Register an application in the Agnic Dashboard, obtain a client ID (and secret if confidential), then run the OAuth 2.0 authorization code flow as described.
  name: OAuth2
  scopes:
  - payments:sign
  - balance:read
  - transactions:read
  token_url: https://api.agnic.ai/oauth/token
  type: oauth2
slug: agnic-ai-authentication
source_filename: agnic-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agnic.ai/docs/api-reference/oauth.mdx
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agnic.ai/docs/api-reference/oauth.mdx\nsources:\n- https://docs.agnic.ai/docs/api-reference/oauth.mdx\n- https://docs.agnic.ai/docs/authentication/api-tokens.mdx\n- https://docs.agnic.ai/docs/authentication.mdx\n- https://docs.agnic.ai/docs/authentication/oauth2.mdx\ndescription: Authentication methods for Agnic APIs\nschemes:\n- type: apiKey\n  name: API Token\n  evidence: 'Include the token in the `X-Agnic-Token` header:'\n  location: header\n  header: X-Agnic-Token\n  how_to_obtain: Generate token via Agnic Dashboard → Connect App → Generate Token (see \"Creating a Token\" section).\n- type: oauth2\n  name: OAuth2\n  evidence: Redirect users to our authorization endpoint. Include PKCE for any non-confidential client.\n  token_url: https://api.agnic.ai/oauth/token\n  authorize_url: https://api.agnic.ai/oauth/authorize\n  scopes:\n  - payments:sign\n  - balance:read\n\
  \  - transactions:read\n  how_to_obtain: Register an application in the Agnic Dashboard, obtain a client ID (and secret if confidential), then run the OAuth 2.0 authorization\n    code flow as described.\ndocs: https://docs.agnic.ai/docs/api-reference/oauth.mdx\n"
source_yaml_url: https://artifacts.apis.io/agnic-ai/authentication/agnic-ai-authentication.yml
summary_line: 2 schemes
tags:
- Agent Wallet
- Payment Infrastructure
- AI Commerce
- Verifiable Credentials
- API Monetization
- Service Discovery
---
