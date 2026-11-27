---
anonymous_access: false
api_key_in: []
api_specs:
- filename: certifier-io-credential-interactions-api-openapi.yml
  format: yaml
  label: Certifier Credential Interactions API
  slug: certifier-io-credential-interactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certifier-io/openapi/certifier-io-credential-interactions-api-openapi.yml
- filename: certifier-io-credential-templates-api-openapi.yml
  format: yaml
  label: Certifier Credential Templates API
  slug: certifier-io-credential-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certifier-io/openapi/certifier-io-credential-templates-api-openapi.yml
- filename: certifier-io-credentials-api-openapi.yml
  format: yaml
  label: Certifier Credentials API
  slug: certifier-io-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certifier-io/openapi/certifier-io-credentials-api-openapi.yml
- filename: certifier-io-design-templates-api-openapi.yml
  format: yaml
  label: Certifier Design Templates API
  slug: certifier-io-design-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certifier-io/openapi/certifier-io-design-templates-api-openapi.yml
auth_types: []
description: Authentication methods for Certifier API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Certifier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Certifier declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Certifier
provider_slug: certifier-io
scheme_count: 2
schemes:
- evidence: The Certifier MCP server uses the standard OAuth authorization code flow for remote MCP servers.
  how_to_obtain: Clients start the OAuth authorization code flow via the discovery document at https://api.certifier.io/.well-known/oauth-authorization-server; no pre‑registered client ID is required.
  name: OAuth2
  scopes:
  - mcp:read
  - mcp:write
  type: oauth2
- evidence: Provide your access token in the Authorization header with Bearer auth-scheme.
  header: Authorization
  how_to_obtain: Access tokens are issued through the OAuth flow described above and can be viewed in the Certifier Dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: certifier-io-authentication
source_filename: certifier-io-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.certifier.io/docs/api-reference/mcp-server
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.certifier.io/docs/api-reference/mcp-server\nsources:\n- https://developers.certifier.io/docs/api-reference/mcp-server\n- https://developers.certifier.io/docs/api-reference/credentials/list-credentials\n- https://developers.certifier.io/docs/api-reference/credentials/get-a-credential\n- https://developers.certifier.io/docs/api-reference/credentials/get-credential-design-templates\ndescription: Authentication methods for Certifier API\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: The Certifier MCP server uses the standard OAuth authorization code flow for remote MCP servers.\n  scopes:\n  - mcp:read\n  - mcp:write\n  how_to_obtain: Clients start the OAuth authorization code flow via the discovery document at https://api.certifier.io/.well-known/oauth-authorization-server;\n    no pre‑registered client ID is required.\n- type: http-bearer\n  name: Bearer\n\
  \  evidence: Provide your access token in the Authorization header with Bearer auth-scheme.\n  location: header\n  header: Authorization\n  how_to_obtain: Access tokens are issued through the OAuth flow described above and can be viewed in the Certifier Dashboard.\ndocs: https://developers.certifier.io/docs/api-reference/mcp-server\n"
source_yaml_url: https://artifacts.apis.io/certifier-io/authentication/certifier-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Certificate
- Artificial Intelligence
- Automation
- Credentials
---
