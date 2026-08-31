---
api_key_in:
- header
api_specs:
- filename: browser-use-api-v4-openapi.json
  format: json
  label: Browser Use Public API v4
  slug: browser-use-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v4-openapi.json
- filename: browser-use-api-v3-openapi.json
  format: json
  label: Browser Use Public API v3
  slug: browser-use-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v3-openapi.json
- filename: browser-use-api-v2-openapi.json
  format: json
  label: Browser Use Public API v2
  slug: browser-use-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v2-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Browser Use Authentication
name_suffix: Authentication
oauth_flows: []
overview: Browser Use secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Browser Use
provider_slug: browser-use
scheme_count: 2
schemes:
- applies_to:
  - https://api.browser-use.com/api/v4
  - https://api.browser-use.com/api/v3
  - https://api.browser-use.com/api/v2
  - https://api.browser-use.com/mcp
  - https://api.browser-use.com/v3/mcp
  in: header
  issued_at: https://cloud.browser-use.com/settings?tab=api-keys&new=1
  key_prefix: bu_
  name: APIKeyHeader
  parameter: X-Browser-Use-API-Key
  sources:
  - openapi/browser-use-api-v2-openapi.json
  - openapi/browser-use-api-v3-openapi.json
  - openapi/browser-use-api-v4-openapi.json
  - https://browser-use.com/auth.md
  type: apiKey
- applies_to:
  - https://api.browser-use.com/mcp
  authorization_endpoint: https://api.browser-use.com/oauth/authorize
  grant_types:
  - authorization_code
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://api.browser-use.com
  metadata: well-known/browser-use-oauth-authorization-server.json
  name: BrowserUseOAuth
  pkce:
  - S256
  protected_resource: well-known/browser-use-oauth-protected-resource.json
  registration_endpoint: https://api.browser-use.com/oauth/register
  revocation_endpoint: https://api.browser-use.com/oauth/revoke
  scopes:
  - mcp
  sources:
  - https://browser-use.com/.well-known/oauth-authorization-server
  - https://api.browser-use.com/.well-known/oauth-protected-resource
  - https://browser-use.com/auth.md
  token_endpoint: https://api.browser-use.com/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: browser-use-authentication
source_filename: browser-use-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://browser-use.com/auth.md\ndocs: https://browser-use.com/auth.md\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    Browser Use publishes two authentication paths. The REST APIs (v2, v3, v4) and both Cloud SDKs use\n    a project API key in the X-Browser-Use-API-Key header; keys are prefixed bu_ and are minted in the\n    Cloud dashboard. The hosted MCP resource is additionally protected by an OAuth 2.0 authorization\n    server that advertises Authorization Code with PKCE and Device Authorization, dynamic client\n    registration, and a single published scope, mcp.\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Browser-Use-API-Key\n  key_prefix: bu_\n  issued_at: https://cloud.browser-use.com/settings?tab=api-keys&new=1\n  applies_to:\n  - https://api.browser-use.com/api/v4\n  - https://api.browser-use.com/api/v3\n  - https://api.browser-use.com/api/v2\n\
  \  - https://api.browser-use.com/mcp\n  - https://api.browser-use.com/v3/mcp\n  sources:\n  - openapi/browser-use-api-v2-openapi.json\n  - openapi/browser-use-api-v3-openapi.json\n  - openapi/browser-use-api-v4-openapi.json\n  - https://browser-use.com/auth.md\n- name: BrowserUseOAuth\n  type: oauth2\n  applies_to:\n  - https://api.browser-use.com/mcp\n  metadata: well-known/browser-use-oauth-authorization-server.json\n  protected_resource: well-known/browser-use-oauth-protected-resource.json\n  issuer: https://api.browser-use.com\n  authorization_endpoint: https://api.browser-use.com/oauth/authorize\n  token_endpoint: https://api.browser-use.com/oauth/token\n  registration_endpoint: https://api.browser-use.com/oauth/register\n  revocation_endpoint: https://api.browser-use.com/oauth/revoke\n  grant_types:\n  - authorization_code\n  - urn:ietf:params:oauth:grant-type:device_code\n  pkce:\n  - S256\n  scopes:\n  - mcp\n  token_endpoint_auth_methods:\n  - none\n  sources:\n  - https://browser-use.com/.well-known/oauth-authorization-server\n\
  \  - https://api.browser-use.com/.well-known/oauth-protected-resource\n  - https://browser-use.com/auth.md\nguidance:\n  published: >-\n    \"Do not put API keys in prompts, source control, browser-delivered code, or logs. Isolate keys by\n    environment, store them in a secret manager, and revoke keys that are no longer needed.\"\n  source: https://browser-use.com/auth.md\ngaps:\n- >-\n  The OpenAPI documents declare only the APIKeyHeader scheme; the OAuth 2.0 path is documented in\n  auth.md and in the well-known metadata but is not represented in any securityScheme.\n- >-\n  No finer-grained REST scopes are advertised. Browser Use states this explicitly: \"Finer-grained REST\n  API OAuth scopes are not currently advertised by the public authorization metadata.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/authentication/browser-use-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- AI Automation
- Browser Automation
- Web Agents
- Web Scraping
- Headless Browsers
- Agent Infrastructure
- Model Context Protocol
- Cloud Browsers
---
