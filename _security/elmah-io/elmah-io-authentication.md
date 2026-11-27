---
anonymous_access: false
api_key_in: []
api_specs:
- filename: elmah-io-v3-openapi.json
  format: json
  label: elmah.io API V3 API
  slug: elmah-io-api-v3-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elmah-io/openapi/_original/elmah-io-v3-openapi.json
auth_types: []
description: Authentication on elmah.io uses API keys passed as Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: elmah.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: elmah.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: elmah.io
provider_slug: elmah-io
scheme_count: 1
schemes:
- evidence: Pass your API key in the Authorization header as a Bearer token on every request to https://mcp.elmah.io/mcp.
  header: Authorization
  how_to_obtain: API keys are available on the Organization Settings view or the Install tab on the Log Settings screen.
  location: header
  name: API Key
  type: http-bearer
slug: elmah-io-authentication
source_filename: elmah-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.elmah.io/authentication/
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.elmah.io/authentication/\nsources:\n- https://docs.elmah.io/authentication/\n- https://docs.elmah.io/call-mcp-server-using-api-key/\n- https://docs.elmah.io/\n- https://docs.elmah.io/setup-mcp-server/\ndescription: Authentication on elmah.io uses API keys passed as Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Pass your API key in the Authorization header as a Bearer token on every request to https://mcp.elmah.io/mcp.\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are available on the Organization Settings view or the Install tab on the Log Settings screen.\nnote: OAuth2 is mentioned for MCP server UI login, but no token or authorize URLs are provided in the documentation, so no OAuth2 flow details\n  are captured.\ndocs: https://docs.elmah.io/authentication/\n"
source_yaml_url: https://artifacts.apis.io/elmah-io/authentication/elmah-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Logging
- Monitoring
- .NET
- Error Tracking
- Cloud
---
