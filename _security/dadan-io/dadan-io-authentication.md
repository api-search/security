---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dadan-io-openapi-generated.yml
  format: yaml
  label: Dadan Recording Request API
  slug: recording-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dadan-io/openapi/_ae-authored/dadan-io-openapi-generated.yml
auth_types:
- apiKey
- oauth2
- publicAppId
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Dadan Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dadan secures its APIs with apiKey, oauth2, and publicAppId across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dadan
provider_slug: dadan-io
scheme_count: 3
schemes:
- applies_to: Recording Request API (app.dadan.io/api/v1/usedadan/requestrecording)
  description: 'API key copied from Account & Settings > Developers (Developer Settings), where the API must also be enabled. Docs: "Do not use the Authorization tab; the API uses a custom header instead."'
  in: header
  name: X-Dadan-API-Key
  sources:
  - https://kb.dadan.io/docs/dadan-recording-request-api-simplified-guide
  - openapi/_ae-authored/dadan-io-openapi-generated.yml
  type: apiKey
- applies_to: Dadan MCP (https://mcp.dadan.io/mcp)
  authorization_server: https://mcp.dadan.io
  description: 'Docs: "You don''t need an API key: when you''re asked, sign in with your Dadan account." Grant types, PKCE method and scopes read from the published OAuth discovery documents (HTTP 200).'
  dynamic_client_registration: https://mcp.dadan.io/oauth/register
  grant_types:
  - authorization_code
  - refresh_token
  name: Dadan MCP OAuth
  pkce: S256
  scopes:
  - dadan:full
  - dadan:read
  sources:
  - https://kb.dadan.io/docs/use-dadan-with-your-ai-assistant-mcp
  - https://mcp.dadan.io/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  type: oauth2
- applies_to: Record SDK (browser)
  description: 'The SDK requests a short-lived upload token with a public app ID; Dadan issues it only when the page origin is on the app''s allowed-origins list. Docs: "The public app ID is all the page needs. Your Dadan API key is never used in the browser." Public apps are included on the Lite, Pro and Business plans.'
  name: Public app ID
  sources:
  - https://kb.dadan.io/docs/dadan-record-sdk-overview
  - https://kb.dadan.io/docs/dadan-record-sdk-production-checklist
  type: publicAppId
slug: dadan-io-authentication
source_filename: dadan-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://kb.dadan.io/docs/dadan-recording-request-api-simplified-guide\n- https://kb.dadan.io/docs/use-dadan-with-your-ai-assistant-mcp\n- https://kb.dadan.io/docs/dadan-record-sdk-overview\n- https://mcp.dadan.io/.well-known/oauth-protected-resource\n- https://mcp.dadan.io/.well-known/oauth-authorization-server\ndocs: https://kb.dadan.io/docs/dadan-recording-request-api-simplified-guide\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - publicAppId\nschemes:\n- name: X-Dadan-API-Key\n  type: apiKey\n  in: header\n  applies_to: Recording Request API (app.dadan.io/api/v1/usedadan/requestrecording)\n  description: 'API key copied from Account & Settings > Developers (Developer Settings), where the API must also\n    be enabled. Docs: \"Do not use the Authorization tab; the API uses a custom header instead.\"'\n  sources:\n  - https://kb.dadan.io/docs/dadan-recording-request-api-simplified-guide\n  - openapi/_ae-authored/dadan-io-openapi-generated.yml\n\
  - name: Dadan MCP OAuth\n  type: oauth2\n  applies_to: Dadan MCP (https://mcp.dadan.io/mcp)\n  grant_types:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  token_endpoint_auth_methods:\n  - none\n  dynamic_client_registration: https://mcp.dadan.io/oauth/register\n  authorization_server: https://mcp.dadan.io\n  scopes:\n  - dadan:full\n  - dadan:read\n  description: 'Docs: \"You don''t need an API key: when you''re asked, sign in with your Dadan account.\" Grant types,\n    PKCE method and scopes read from the published OAuth discovery documents (HTTP 200).'\n  sources:\n  - https://kb.dadan.io/docs/use-dadan-with-your-ai-assistant-mcp\n  - https://mcp.dadan.io/.well-known/oauth-authorization-server\n- name: Public app ID\n  type: publicAppId\n  applies_to: Record SDK (browser)\n  description: 'The SDK requests a short-lived upload token with a public app ID; Dadan issues it only when the\n    page origin is on the app''s allowed-origins list. Docs: \"The public app ID is all\
  \ the page needs. Your Dadan\n    API key is never used in the browser.\" Public apps are included on the Lite, Pro and Business plans.'\n  sources:\n  - https://kb.dadan.io/docs/dadan-record-sdk-overview\n  - https://kb.dadan.io/docs/dadan-record-sdk-production-checklist\n"
source_yaml_url: https://artifacts.apis.io/dadan-io/authentication/dadan-io-authentication.yml
summary_line: apiKey/oauth2/publicAppId · 3 schemes
tags:
- Company
- Video
- Screen Recording
- Video Hosting
- Video Analytics
- MCP
- AI Agents
---
