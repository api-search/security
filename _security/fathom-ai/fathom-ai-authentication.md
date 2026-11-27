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
description: Authentication methods for Fathom API as documented.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Fathom AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fathom AI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Fathom AI
provider_slug: fathom-ai
scheme_count: 3
schemes:
- evidence: Authenticate with the Fathom SDKs using API keys
  how_to_obtain: Configure your redirects and receive your OAuth credentials. (2 mins) – see the Register an OAuth App page for the API key.
  name: apiKeyAuth
  type: apiKey
- evidence: Bearer Token Authentication
  how_to_obtain: Provide a bearer token string (e.g., "YOUR_BEARER_TOKEN") when constructing the SDK client.
  name: bearerAuth
  type: http-bearer
- evidence: Both TypeScript and Python SDKs support OAuth 2.0 authentication for building integrations that can be installed by multiple Fathom accounts.
  how_to_obtain: Register an OAuth app to receive a client ID and client secret, then use the SDK’s getAuthorizationUrl method to start the flow.
  name: oauth2
  scopes:
  - public_api
  token_url: https://api.fathom.ai/external/v1/oauth2/token
  type: oauth2
slug: fathom-ai-authentication
source_filename: fathom-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.fathom.ai/oauth.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.fathom.ai/oauth.md\nsources:\n- https://developers.fathom.ai/oauth.md\n- https://developers.fathom.ai/sdks/authentication.md\n- https://developers.fathom.ai/sdks/oauth.md\n- https://developers.fathom.ai/oauth\ndescription: Authentication methods for Fathom API as documented.\nschemes:\n- type: apiKey\n  name: apiKeyAuth\n  evidence: Authenticate with the Fathom SDKs using API keys\n  how_to_obtain: Configure your redirects and receive your OAuth credentials. (2 mins) – see the Register an OAuth App page for the API key.\n- type: http-bearer\n  name: bearerAuth\n  evidence: Bearer Token Authentication\n  how_to_obtain: Provide a bearer token string (e.g., \"YOUR_BEARER_TOKEN\") when constructing the SDK client.\n- type: oauth2\n  name: oauth2\n  evidence: Both TypeScript and Python SDKs support OAuth 2.0 authentication for building integrations that can be installed\
  \ by multiple Fathom\n    accounts.\n  token_url: https://api.fathom.ai/external/v1/oauth2/token\n  scopes:\n  - public_api\n  how_to_obtain: Register an OAuth app to receive a client ID and client secret, then use the SDK’s getAuthorizationUrl method to start the flow.\ndocs: https://developers.fathom.ai/oauth.md\n"
source_yaml_url: https://artifacts.apis.io/fathom-ai/authentication/fathom-ai-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Note Taking
- Collaboration
- Transcription
- Productivity
---
