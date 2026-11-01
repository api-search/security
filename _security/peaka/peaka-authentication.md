---
anonymous_access: false
api_key_in: []
api_specs:
- filename: peaka-api-openapi.json
  format: json
  label: Peaka Gateway API API
  slug: peaka-gateway-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peaka/openapi/_original/peaka-api-openapi.json
auth_types: []
description: 'Peaka supports two authentication mechanisms: OAuth for remote installs and API keys for local installs.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Peaka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peaka declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Peaka
provider_slug: peaka
scheme_count: 2
schemes:
- evidence: When a client connects to `https://mcp.peaka.studio/mcp`, the server returns `401 Unauthorized` with OAuth metadata in the `WWW-Authenticate` header. Your MCP client opens a browser to `mcp.peaka.studio`, you sign in to Peaka, approve the consent screen, and the client receives an access token.
  how_to_obtain: User signs in via browser to `mcp.peaka.studio` and approves consent; the client receives an access token.
  name: Remote OAuth
  type: oauth2
- evidence: The NPM and from-source installs read a Peaka API key from the `PEAKA_API_KEY` environment variable.
  how_to_obtain: Generate an API key via the Peaka settings page (see “How to generate API Keys”) and provide it in the `PEAKA_API_KEY` environment variable.
  location: env
  name: PEAKA_API_KEY
  type: apiKey
slug: peaka-authentication
source_filename: peaka-authentication.yml
source_heading: Authentication Profile
source_url: https://www.peaka.com/docs/cookbook/how-to-create-peaka-rest-api-catalog-with-authentication/how-to-create-peaka-rest-api-catalog-with-authentication.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.peaka.com/docs/cookbook/how-to-create-peaka-rest-api-catalog-with-authentication/how-to-create-peaka-rest-api-catalog-with-authentication.md\nsources:\n- https://www.peaka.com/docs/cookbook/how-to-create-peaka-rest-api-catalog-with-authentication/how-to-create-peaka-rest-api-catalog-with-authentication.md\n- https://www.peaka.com/docs/cookbook/how-to-generate-api-keys/how-to-generate-api-keys.md\n- https://www.peaka.com/docs/cookbook/how-to-manage-partner-api-key/how-to-manage-partner-api-key.md\n- https://www.peaka.com/docs/mcp/authentication/authentication.md\ndescription: 'Peaka supports two authentication mechanisms: OAuth for remote installs and API keys for local installs.'\nschemes:\n- type: oauth2\n  name: Remote OAuth\n  evidence: When a client connects to `https://mcp.peaka.studio/mcp`, the server returns `401 Unauthorized` with OAuth metadata in the `WWW-Authenticate`\n\
  \    header. Your MCP client opens a browser to `mcp.peaka.studio`, you sign in to Peaka, approve the consent screen, and the client receives an\n    access token.\n  how_to_obtain: User signs in via browser to `mcp.peaka.studio` and approves consent; the client receives an access token.\n- type: apiKey\n  name: PEAKA_API_KEY\n  evidence: The NPM and from-source installs read a Peaka API key from the `PEAKA_API_KEY` environment variable.\n  location: env\n  how_to_obtain: Generate an API key via the Peaka settings page (see “How to generate API Keys”) and provide it in the `PEAKA_API_KEY` environment\n    variable.\ndocs: https://www.peaka.com/docs/cookbook/how-to-create-peaka-rest-api-catalog-with-authentication/how-to-create-peaka-rest-api-catalog-with-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/peaka/authentication/peaka-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data Integration
- AI-Ready
- Governance
- Analytics
---
