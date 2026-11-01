---
anonymous_access: false
api_key_in: []
api_specs:
- filename: plainrouter-actiondryrunapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Dry Run API
  slug: plainrouter-actiondryrunapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-actiondryrunapi-api-openapi.yml
- filename: plainrouter-actionproposalapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Proposal API
  slug: plainrouter-actionproposalapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-actionproposalapi-api-openapi.yml
- filename: plainrouter-actionreadapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Read API
  slug: plainrouter-actionreadapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-actionreadapi-api-openapi.yml
- filename: plainrouter-actionruleapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Rule API
  slug: plainrouter-actionruleapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-actionruleapi-api-openapi.yml
- filename: plainrouter-adtestapi-api-openapi.yml
  format: yaml
  label: Plainrouter Ad Test API
  slug: plainrouter-adtestapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-adtestapi-api-openapi.yml
- filename: plainrouter-agentcontext-api-openapi.yml
  format: yaml
  label: Plainrouter Agent Context API
  slug: plainrouter-agentcontext-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-agentcontext-api-openapi.yml
- filename: plainrouter-cookiedeclaration-api-openapi.yml
  format: yaml
  label: Plainrouter Cookie Declaration API
  slug: plainrouter-cookiedeclaration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-cookiedeclaration-api-openapi.yml
- filename: plainrouter-creative-api-openapi.yml
  format: yaml
  label: Plainrouter Creative API
  slug: plainrouter-creative-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-creative-api-openapi.yml
- filename: plainrouter-deploymentplan-api-openapi.yml
  format: yaml
  label: Plainrouter Deployment Plan API
  slug: plainrouter-deploymentplan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-deploymentplan-api-openapi.yml
- filename: plainrouter-draftbatchfileimport-api-openapi.yml
  format: yaml
  label: Plainrouter Draft Batch File Import API
  slug: plainrouter-draftbatchfileimport-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-draftbatchfileimport-api-openapi.yml
- filename: plainrouter-event-api-openapi.yml
  format: yaml
  label: Plainrouter Event API
  slug: plainrouter-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-event-api-openapi.yml
- filename: plainrouter-launchpolicy-api-openapi.yml
  format: yaml
  label: Plainrouter Launch Policy API
  slug: plainrouter-launchpolicy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-launchpolicy-api-openapi.yml
- filename: plainrouter-metainventoryexposure-api-openapi.yml
  format: yaml
  label: Plainrouter Meta Inventory Exposure API
  slug: plainrouter-metainventoryexposure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-metainventoryexposure-api-openapi.yml
- filename: plainrouter-operations-api-openapi.yml
  format: yaml
  label: Plainrouter Operations API
  slug: plainrouter-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-operations-api-openapi.yml
- filename: plainrouter-sandbox-api-openapi.yml
  format: yaml
  label: Plainrouter Sandbox API
  slug: plainrouter-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plainrouter/openapi/plainrouter-sandbox-api-openapi.yml
auth_types: []
description: Authentication methods for Plainrouter APIs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Plainrouter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plainrouter declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Plainrouter
provider_slug: plainrouter
scheme_count: 3
schemes:
- evidence: Send the Server secret as a bearer token to the server-side Conversion API at https://plainrouter.com/api/v1
  header: Authorization
  how_to_obtain: Create the Server secret in Settings → Workspace → Server secret for the workspace
  location: header
  name: Server secret
  type: http-bearer
- evidence: 'Send it as a bearer token, kept in an environment variable or secret manager:'
  header: Authorization
  how_to_obtain: A workspace owner or member creates a key in Settings → Workspace keys
  location: header
  name: Workspace key
  type: http-bearer
- authorize_url: https://plainrouter.com/oauth2/authorize
  evidence: OAuth clients connect to https://plainrouter.com/mcp, open the browser authorization flow, and let the human user choose exactly one advertising account and Read or Write access.
  flows:
  - authorization_code
  how_to_obtain: Register a public OAuth client (POST /oauth/register) and perform the Authorization Code with PKCE flow
  name: MCP OAuth 2.1
  scopes:
  - mcp:use
  type: oauth2
slug: plainrouter-authentication
source_filename: plainrouter-authentication.yml
source_heading: Authentication Profile
source_url: https://plainrouter.com/docs/api/authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://plainrouter.com/docs/api/authentication\nsources:\n- https://plainrouter.com/docs/api/authentication\n- https://plainrouter.com/auth.md\n- https://plainrouter.com/api/v1/sandbox.md\n- https://plainrouter.com/api/v1/sandbox\ndescription: Authentication methods for Plainrouter APIs\nschemes:\n- type: http-bearer\n  name: Server secret\n  evidence: Send the Server secret as a bearer token to the server-side Conversion API at https://plainrouter.com/api/v1\n  location: header\n  header: Authorization\n  how_to_obtain: Create the Server secret in Settings → Workspace → Server secret for the workspace\n- type: http-bearer\n  name: Workspace key\n  evidence: 'Send it as a bearer token, kept in an environment variable or secret manager:'\n  location: header\n  header: Authorization\n  how_to_obtain: A workspace owner or member creates a key in Settings → Workspace keys\n- type:\
  \ oauth2\n  name: MCP OAuth 2.1\n  evidence: OAuth clients connect to https://plainrouter.com/mcp, open the browser authorization flow, and let the human user choose exactly one\n    advertising account and Read or Write access.\n  flows:\n  - authorization_code\n  authorize_url: https://plainrouter.com/oauth2/authorize\n  scopes:\n  - mcp:use\n  how_to_obtain: Register a public OAuth client (POST /oauth/register) and perform the Authorization Code with PKCE flow\ndocs: https://plainrouter.com/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/plainrouter/authentication/plainrouter-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Advertising
- Developer Tools
- PaidAds
---
