---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chamelio-openapi-generated.yml
  format: yaml
  label: Chamelio API
  slug: chamelio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chamelio/openapi/_ae-authored/chamelio-openapi-generated.yml
auth_types: []
description: Authentication methods for Chamelio API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chamelio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chamelio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chamelio
provider_slug: chamelio
scheme_count: 2
schemes:
- evidence: 'Include your API key in every request using the `X-API-Key` header:'
  header: X-API-Key
  how_to_obtain: 'Generate an API key from the Chamelio web application: go to Settings > Developer, open the API Key tab and click Create API Key.'
  location: header
  name: API Key
  type: apiKey
- authorize_url: https://platform.chamelio.ai/oauth/authorize
  evidence: 'Send the access token as a bearer token:'
  header: Authorization
  how_to_obtain: 'Register an application in the Chamelio web application, then follow the OAuth 2.1 PKCE flow: send the user to the `/oauth/authorize` endpoint to obtain an authorization code, and exchange the code at `/oauth/token` for an access token.'
  location: header
  name: OAuth App
  scopes:
  - workflows:read
  - workflows:write
  - tasks:read
  - tasks:write
  - files:read
  - users:read
  - users:write
  - sor:read
  - sor:write
  - clickwrap:read
  - clickwrap:write
  - agent:write
  token_url: https://platform.chamelio.ai/oauth/token
  type: oauth2
slug: chamelio-authentication
source_filename: chamelio-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.chamelio.ai/api-reference/introduction.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.chamelio.ai/api-reference/introduction.md\nsources:\n- https://docs.chamelio.ai/api-reference/introduction.md\n- https://docs.chamelio.ai/api-reference/api-keys.md\n- https://docs.chamelio.ai/api-reference/oauth-apps.md\n- https://docs.chamelio.ai/api-reference/oauth/applications.md\ndescription: Authentication methods for Chamelio API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Include your API key in every request using the `X-API-Key` header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: 'Generate an API key from the Chamelio web application: go to Settings > Developer, open the API Key tab and click Create API\n    Key.'\n- type: oauth2\n  name: OAuth App\n  evidence: 'Send the access token as a bearer token:'\n  location: header\n  header: Authorization\n  token_url: https://platform.chamelio.ai/oauth/token\n  authorize_url: https://platform.chamelio.ai/oauth/authorize\n\
  \  scopes:\n  - workflows:read\n  - workflows:write\n  - tasks:read\n  - tasks:write\n  - files:read\n  - users:read\n  - users:write\n  - sor:read\n  - sor:write\n  - clickwrap:read\n  - clickwrap:write\n  - agent:write\n  how_to_obtain: 'Register an application in the Chamelio web application, then follow the OAuth 2.1 PKCE flow: send the user to the `/oauth/authorize`\n    endpoint to obtain an authorization code, and exchange the code at `/oauth/token` for an access token.'\ndocs: https://docs.chamelio.ai/api-reference/introduction.md\n"
source_yaml_url: https://artifacts.apis.io/chamelio/authentication/chamelio-authentication.yml
summary_line: 2 schemes
tags:
- Company
- LegalTech
- SaaS
- Contracts
- Compliance
---
