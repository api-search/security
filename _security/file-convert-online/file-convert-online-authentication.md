---
anonymous_access: false
api_key_in: []
api_specs:
- filename: file-convert-online-mcp-openapi.json
  format: json
  label: File Convert Online — Public Agent API Mcp API
  slug: file-convert-online-public-agent-api-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/file-convert-online/openapi/_original/file-convert-online-mcp-openapi.json
auth_types: []
description: FileConvert uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FileConvert Authentication
name_suffix: Authentication
oauth_flows: []
overview: FileConvert declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FileConvert
provider_slug: file-convert-online
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer fc_live_YOUR_KEY'
  header: Authorization
  how_to_obtain: Create an API key via the account page (file-convert.online/account/api-keys) or by POST /api/identity/v1/api-keys using a login access token.
  location: header
  name: Authorization
  type: http-bearer
slug: file-convert-online-authentication
source_filename: file-convert-online-authentication.yml
source_heading: Authentication Profile
source_url: https://file-convert.online/blog/file-convert-mcp-server-quickstart
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://file-convert.online/blog/file-convert-mcp-server-quickstart\nsources:\n- https://file-convert.online/blog/file-convert-mcp-server-quickstart\ndescription: FileConvert uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer fc_live_YOUR_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the account page (file-convert.online/account/api-keys) or by POST /api/identity/v1/api-keys using a login\n    access token.\nnote: No OAuth2 flows, API key is the only authentication method described.\ndocs: https://file-convert.online/blog/file-convert-mcp-server-quickstart\n"
source_yaml_url: https://artifacts.apis.io/file-convert-online/authentication/file-convert-online-authentication.yml
summary_line: 1 scheme
tags:
- Company
- File Conversion
- Free
- Online
- Utility
- Converter
---
