---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcpbundles-local-runtime-api-openapi.yml
  format: yaml
  label: MCPBundles Local Runtime API
  slug: mcpbundles-local-runtime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpbundles/openapi/mcpbundles-local-runtime-api-openapi.yml
- filename: mcpbundles-tunnel-api-openapi.yml
  format: yaml
  label: MCPBundles Tunnel API
  slug: mcpbundles-tunnel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpbundles/openapi/mcpbundles-tunnel-api-openapi.yml
- filename: mcpbundles-graph-ql-api-openapi.yml
  format: yaml
  label: MCPBundles Graph QL API
  slug: mcpbundles-graph-ql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpbundles/openapi/mcpbundles-graph-ql-api-openapi.yml
auth_types: []
description: MCPBundles provides workspace API keys for programmatic access. Clients must send the key in a request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mcpbundles Authentication
name_suffix: Authentication
oauth_flows: []
overview: MCPBundles declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MCPBundles
provider_slug: mcpbundles
scheme_count: 1
schemes:
- evidence: 'Authenticate GraphQL requests using the X-API-Key header:'
  header: X-API-Key
  how_to_obtain: Create a workspace API key in the workspace settings, copy it immediately; keys start with mb_.
  location: header
  name: Workspace API Key
  type: apiKey
slug: mcpbundles-authentication
source_filename: mcpbundles-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mcpbundles.com/docs/how-to/using-api-keys
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mcpbundles.com/docs/how-to/using-api-keys\nsources:\n- https://www.mcpbundles.com/docs/how-to/using-api-keys\n- https://www.mcpbundles.com/docs/how-to/setting-up-credentials\n- https://www.mcpbundles.com/docs/guides/user/credential-validation\n- https://www.mcpbundles.com/docs/guides/user/managing-credentials\ndescription: MCPBundles provides workspace API keys for programmatic access. Clients must send the key in a request header.\nschemes:\n- type: apiKey\n  name: Workspace API Key\n  evidence: 'Authenticate GraphQL requests using the X-API-Key header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a workspace API key in the workspace settings, copy it immediately; keys start with mb_.\nnote: No other authentication schemes (OAuth2, http-bearer, etc.) are documented on the referenced pages.\ndocs: https://www.mcpbundles.com/docs/how-to/using-api-keys\n"
source_yaml_url: https://artifacts.apis.io/mcpbundles/authentication/mcpbundles-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Directory
- ManagedCloudPlatforms
- Tools
- Integration
---
