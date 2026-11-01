---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentfabric-dev-openapi-generated.yml
  format: yaml
  label: agentfabric-dev API
  slug: agentfabric-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentfabric-dev/openapi/_ae-authored/agentfabric-dev-openapi-generated.yml
auth_types: []
description: Authentication methods documented for agentfabric-dev
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Agentfabric Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: agentfabric-dev declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: agentfabric-dev
provider_slug: agentfabric-dev
scheme_count: 5
schemes:
- evidence: 'x-api-key: ak_… or Authorization: Bearer ak_…'
  header: x-api-key
  how_to_obtain: Returned once on create/signup/rotate ( ak_… ) via the signup endpoint or create_tenant tool.
  location: header
  name: x-api-key
  scopes:
  - admin
  - consumer
  type: apiKey
- evidence: 'x-api-key: ak_… or Authorization: Bearer ak_…'
  header: Authorization
  how_to_obtain: Returned once on create/signup/rotate ( ak_… ) via the signup endpoint or create_tenant tool.
  location: header
  name: Authorization
  scopes:
  - admin
  - consumer
  type: http-bearer
- evidence: Cognito email/password → bearer access token (or x-access-token )
  header: Authorization
  how_to_obtain: Sign in via Cognito using email and password to receive a bearer access token.
  location: header
  name: Authorization
  type: http-bearer
- evidence: Cognito email/password → bearer access token (or x-access-token )
  header: x-access-token
  how_to_obtain: Sign in via Cognito using email and password to receive an access token placed in the x-access-token header.
  location: header
  name: x-access-token
  type: http-bearer
- evidence: Personal link with auth code ( rrc_… )
  how_to_obtain: Reviewer receives a personal link containing an auth code (rrc_…) via email.
  location: query
  name: authCode
  type: other
slug: agentfabric-dev-authentication
source_filename: agentfabric-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://agentfabric.dev/docs/concepts
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentfabric.dev/docs/concepts\nsources:\n- https://agentfabric.dev/docs/concepts\n- https://agentfabric.dev/docs/mcp\n- https://agentfabric.dev/docs\ndescription: Authentication methods documented for agentfabric-dev\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'x-api-key: ak_… or Authorization: Bearer ak_…'\n  location: header\n  header: x-api-key\n  scopes:\n  - admin\n  - consumer\n  how_to_obtain: Returned once on create/signup/rotate ( ak_… ) via the signup endpoint or create_tenant tool.\n- type: http-bearer\n  name: Authorization\n  evidence: 'x-api-key: ak_… or Authorization: Bearer ak_…'\n  location: header\n  header: Authorization\n  scopes:\n  - admin\n  - consumer\n  how_to_obtain: Returned once on create/signup/rotate ( ak_… ) via the signup endpoint or create_tenant tool.\n- type: http-bearer\n  name: Authorization\n  evidence: Cognito email/password\
  \ → bearer access token (or x-access-token )\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in via Cognito using email and password to receive a bearer access token.\n- type: http-bearer\n  name: x-access-token\n  evidence: Cognito email/password → bearer access token (or x-access-token )\n  location: header\n  header: x-access-token\n  how_to_obtain: Sign in via Cognito using email and password to receive an access token placed in the x-access-token header.\n- type: other\n  name: authCode\n  evidence: Personal link with auth code ( rrc_… )\n  location: query\n  how_to_obtain: Reviewer receives a personal link containing an auth code (rrc_…) via email.\nnote: No OAuth2 flows are documented on the pages.\ndocs: https://agentfabric.dev/docs/concepts\n"
source_yaml_url: https://artifacts.apis.io/agentfabric-dev/authentication/agentfabric-dev-authentication.yml
summary_line: 5 schemes
tags:
- Company
- AI
- HumanReview
- MCP
- REST
- Automation
---
