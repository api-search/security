---
anonymous_access: false
api_key_in: []
api_specs:
- filename: augments-dev-2026-07-28-openapi-generated.yml
  format: yaml
  label: augments-dev 2026 07 28 API
  slug: 2026-07-28-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/augments-dev/openapi/_ae-authored/augments-dev-2026-07-28-openapi-generated.yml
- filename: augments-dev-core-openapi-generated.yml
  format: yaml
  label: augments-dev core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/augments-dev/openapi/_ae-authored/augments-dev-core-openapi-generated.yml
- filename: augments-dev-draft-openapi-generated.yml
  format: yaml
  label: augments-dev draft API
  slug: draft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/augments-dev/openapi/_ae-authored/augments-dev-draft-openapi-generated.yml
auth_types: []
description: Authentication schemes for augments-dev
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Augments Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: augments-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: augments-dev
provider_slug: augments-dev
scheme_count: 1
schemes:
- evidence: 'Pass the token in the `Authorization` header of HTTP requests to the MCP server:'
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: Obtain an access token from the authorization server using the client credentials grant (client_id and client_secret or a signed JWT) before connecting to the MCP server.
  location: header
  name: OAuth Client Credentials
  type: http-bearer
slug: augments-dev-authentication
source_filename: augments-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://modelcontextprotocol.io/extensions/auth/oauth-client-credentials.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://modelcontextprotocol.io/extensions/auth/oauth-client-credentials.md\nsources:\n- https://modelcontextprotocol.io/extensions/auth/oauth-client-credentials.md\n- https://modelcontextprotocol.io/registry/authentication.md\n- https://modelcontextprotocol.io/seps/985-align-oauth-20-protected-resource-metadata-with-rf.md\n- https://modelcontextprotocol.io/seps/990-enable-enterprise-idp-policy-controls-during-mcp-o.md\ndescription: Authentication schemes for augments-dev\nschemes:\n- type: http-bearer\n  name: OAuth Client Credentials\n  evidence: 'Pass the token in the `Authorization` header of HTTP requests to the MCP server:'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  how_to_obtain: Obtain an access token from the authorization server using the client credentials grant (client_id and client_secret or a signed\n    JWT) before connecting\
  \ to the MCP server.\ndocs: https://modelcontextprotocol.io/extensions/auth/oauth-client-credentials.md\n"
source_yaml_url: https://artifacts.apis.io/augments-dev/authentication/augments-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- TypeScript
- npm
- Documentation
- CodeExamples
---
