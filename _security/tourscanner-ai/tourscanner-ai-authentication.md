---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for TourScanner AI MCP
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Tourscanner Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: TourScanner AI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: TourScanner AI
provider_slug: tourscanner-ai
scheme_count: 3
schemes:
- evidence: 'Send it as Authorization: Bearer <key> or X-API-Key: <key> . Clients that cannot send headers put it in the URL as ?api_key=<key> .'
  header: Authorization
  how_to_obtain: 'Keys are issued by TourScanner on request: [email protected]'
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'Send it as Authorization: Bearer <key> or X-API-Key: <key> . Clients that cannot send headers put it in the URL as ?api_key=<key> .'
  header: X-API-Key
  how_to_obtain: 'Keys are issued by TourScanner on request: [email protected]'
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Send it as Authorization: Bearer <key> or X-API-Key: <key> . Clients that cannot send headers put it in the URL as ?api_key=<key> .'
  how_to_obtain: 'Keys are issued by TourScanner on request: [email protected]'
  location: query
  name: api_key
  type: apiKey
slug: tourscanner-ai-authentication
source_filename: tourscanner-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://tourscanner.ai/mcp
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tourscanner.ai/mcp\nsources:\n- https://tourscanner.ai/mcp\ndescription: Authentication for TourScanner AI MCP\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Send it as Authorization: Bearer <key> or X-API-Key: <key> . Clients that cannot send headers put it in the URL as ?api_key=<key>\n    .'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Keys are issued by TourScanner on request: [email protected]'\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Send it as Authorization: Bearer <key> or X-API-Key: <key> . Clients that cannot send headers put it in the URL as ?api_key=<key>\n    .'\n  location: header\n  header: X-API-Key\n  how_to_obtain: 'Keys are issued by TourScanner on request: [email protected]'\n- type: apiKey\n  name: api_key\n  evidence: 'Send it as Authorization: Bearer <key> or X-API-Key: <key> . Clients that cannot send\
  \ headers put it in the URL as ?api_key=<key>\n    .'\n  location: query\n  how_to_obtain: 'Keys are issued by TourScanner on request: [email protected]'\ndocs: https://tourscanner.ai/mcp\n"
source_yaml_url: https://artifacts.apis.io/tourscanner-ai/authentication/tourscanner-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Tours
- Activities
- API
- Booking
---
