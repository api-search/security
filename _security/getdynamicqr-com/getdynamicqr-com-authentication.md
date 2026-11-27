---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getdynamicqr-com-openapi-generated.yml
  format: yaml
  label: D-QR API
  slug: getdynamicqr-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getdynamicqr-com/openapi/_ae-authored/getdynamicqr-com-openapi-generated.yml
auth_types: []
description: Authentication methods for D-QR MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: D-QR Authentication
name_suffix: Authentication
oauth_flows: []
overview: D-QR declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: D-QR
provider_slug: getdynamicqr-com
scheme_count: 1
schemes:
- evidence: 'Claude Code is configured from a file rather than a settings screen, so it takes the token route: an entry with "type": "http" , the url , and an Authorization header carrying Bearer and your token.'
  header: Authorization
  how_to_obtain: You make a named token in your dashboard and paste it in beside the address.
  location: header
  name: MCP token
  type: http-bearer
slug: getdynamicqr-com-authentication
source_filename: getdynamicqr-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getdynamicqr.com/blog/whatsapp-qr-codes-customer-support
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getdynamicqr.com/blog/whatsapp-qr-codes-customer-support\nsources:\n- https://getdynamicqr.com/blog/whatsapp-qr-codes-customer-support\n- https://getdynamicqr.com/mcp-setup\ndescription: Authentication methods for D-QR MCP API\nschemes:\n- type: http-bearer\n  name: MCP token\n  evidence: 'Claude Code is configured from a file rather than a settings screen, so it takes the token route: an entry with \"type\": \"http\" ,\n    the url , and an Authorization header carrying Bearer and your token.'\n  location: header\n  header: Authorization\n  how_to_obtain: You make a named token in your dashboard and paste it in beside the address.\nnote: No OAuth flows, apiKey, or other authentication schemes are described on the provided pages.\ndocs: https://getdynamicqr.com/blog/whatsapp-qr-codes-customer-support\n"
source_yaml_url: https://artifacts.apis.io/getdynamicqr-com/authentication/getdynamicqr-com-authentication.yml
summary_line: 1 scheme
tags:
- QR Codes
- Dynamic
- Analytics
- Software-as-a-Service
---
