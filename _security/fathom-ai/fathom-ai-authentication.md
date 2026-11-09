---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fathom-ai-openapi-generated.yml
  format: yaml
  label: Fathom AI API
  slug: fathom-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fathom-ai/openapi/_ae-authored/fathom-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Fathom API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Fathom Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fathom AI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Fathom AI
provider_slug: fathom-ai
scheme_count: 3
schemes:
- evidence: Authenticate with the Fathom SDKs using API keys
  header: X-Api-Key
  how_to_obtain: Generate an API key in the API Access section of your User Settings
  location: header
  name: apiKeyAuth
  type: apiKey
- evidence: Bearer Token Authentication
  header: Authorization
  how_to_obtain: Provide a bearer token (e.g., OAuth access token) to the SDK
  location: header
  name: bearerAuth
  type: http-bearer
- evidence: Both TypeScript and Python SDKs support OAuth 2.0 authentication for building integrations that can be installed by multiple Fathom accounts.
  how_to_obtain: Register an OAuth app to receive client ID and client secret, then use the SDK to generate an authorization URL and exchange the code for tokens
  name: oauth2
  scopes:
  - public_api
  token_url: https://api.fathom.ai/external/v1/oauth2/token
  type: oauth2
slug: fathom-ai-authentication
source_filename: fathom-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.fathom.ai/oauth.md
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.fathom.ai/oauth.md\nsources:\n- https://developers.fathom.ai/oauth.md\n- https://developers.fathom.ai/sdks/authentication.md\n- https://developers.fathom.ai/sdks/oauth.md\n- https://developers.fathom.ai/quickstart.md\ndescription: Authentication methods for Fathom API\nschemes:\n- type: apiKey\n  name: apiKeyAuth\n  evidence: Authenticate with the Fathom SDKs using API keys\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Generate an API key in the API Access section of your User Settings\n- type: http-bearer\n  name: bearerAuth\n  evidence: Bearer Token Authentication\n  location: header\n  header: Authorization\n  how_to_obtain: Provide a bearer token (e.g., OAuth access token) to the SDK\n- type: oauth2\n  name: oauth2\n  evidence: Both TypeScript and Python SDKs support OAuth 2.0 authentication for building integrations that can be installed by multiple\
  \ Fathom\n    accounts.\n  token_url: https://api.fathom.ai/external/v1/oauth2/token\n  scopes:\n  - public_api\n  how_to_obtain: Register an OAuth app to receive client ID and client secret, then use the SDK to generate an authorization URL and exchange\n    the code for tokens\ndocs: https://developers.fathom.ai/oauth.md\n"
source_yaml_url: https://artifacts.apis.io/fathom-ai/authentication/fathom-ai-authentication.yml
summary_line: 3 schemes
tags:
- AI
- Meeting
- Productivity
- Note-taking
- Integration
---
