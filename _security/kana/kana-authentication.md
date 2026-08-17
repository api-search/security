---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Kana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kana declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kana
provider_slug: kana
scheme_count: 2
schemes:
- code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  evidence:
    content_type: application/json; charset=utf-8
    fetched: '2026-08-13'
    http_status: 200
    url: https://apps.kana.ai/.well-known/oauth-authorization-server
  flows:
    authorization_code:
      authorization_url: https://apps.kana.ai/oauth/authorize
      refresh_url: https://apps.kana.ai/oauth/token
      scopes:
      - mcp:read
      - mcp:write
      - kana:read
      - kana:write
      token_url: https://apps.kana.ai/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: oauth2
  introspection_endpoint: https://apps.kana.ai/oauth/introspect
  issuer: https://apps.kana.ai
  note: 'token_endpoint_auth_methods_supported includes "none", and only S256 PKCE is offered — the shape an MCP client uses. The metadata additionally carries "mcp_protocol_version": "2025-03-26".'
  public_clients_supported: true
  registration_endpoint: https://apps.kana.ai/oauth/register
  revocation_endpoint: https://apps.kana.ai/oauth/revoke
  spec: RFC 6749 + RFC 8414 (metadata) + RFC 7636 (PKCE) + RFC 7591 (DCR)
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- applies_to: Kana Skill API (POST /skill/{pipelineid}, /run/*, /file_ul, /file_dl/*)
  evidence:
    fetched: '2026-08-13'
    http_status: 200
    url: https://apps.kana.ai/index.js
  id: apikey
  in: header
  method: derived
  name: x-kana-apikey
  note: 'Read from the OpenAPI 3.0.3 document Kana''s own console bundle generates for a deployed skill (info.title "Kana API"; components.securitySchemes.apikey = {type: apiKey, in: header, name: x-kana-apikey}; every operation carries security: [{apikey: []}] and a documented 401 "Invalid apikey specified"). The generated document is rendered in a Swagger UI inside the signed-in console; it is not published at a public URL, so no spec was saved to openapi/.'
  source: https://apps.kana.ai/index.js
  type: apiKey
slug: kana-authentication
source_filename: kana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://apps.kana.ai/.well-known/oauth-authorization-server\ndocs: null\nhost: https://apps.kana.ai\nsummary: >-\n  Kana's application host runs two distinct authentication models side by side: an\n  OAuth 2.0 authorization server (RFC 8414 metadata served anonymously, PKCE-only,\n  with RFC 7591 dynamic client registration) that fronts the platform's MCP server,\n  and a simple API-key header for the Skill API that a deployed Kana pipeline exposes.\nschemes:\n- id: oauth2\n  type: oauth2\n  spec: RFC 6749 + RFC 8414 (metadata) + RFC 7636 (PKCE) + RFC 7591 (DCR)\n  issuer: https://apps.kana.ai\n  flows:\n    authorization_code:\n      authorization_url: https://apps.kana.ai/oauth/authorize\n      token_url: https://apps.kana.ai/oauth/token\n      refresh_url: https://apps.kana.ai/oauth/token\n      scopes:\n      - mcp:read\n      - mcp:write\n      - kana:read\n      - kana:write\n  grant_types_supported:\n  - authorization_code\n\
  \  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  registration_endpoint: https://apps.kana.ai/oauth/register\n  introspection_endpoint: https://apps.kana.ai/oauth/introspect\n  revocation_endpoint: https://apps.kana.ai/oauth/revoke\n  dynamic_client_registration: true\n  public_clients_supported: true\n  note: >-\n    token_endpoint_auth_methods_supported includes \"none\", and only S256 PKCE is\n    offered — the shape an MCP client uses. The metadata additionally carries\n    \"mcp_protocol_version\": \"2025-03-26\".\n  evidence:\n    url: https://apps.kana.ai/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json; charset=utf-8\n    fetched: '2026-08-13'\n- id: apikey\n  type: apiKey\n  in: header\n  name: x-kana-apikey\n  applies_to: Kana Skill API (POST /skill/{pipelineid}, /run/*, /file_ul, /file_dl/*)\n  method: derived\n\
  \  source: https://apps.kana.ai/index.js\n  note: >-\n    Read from the OpenAPI 3.0.3 document Kana's own console bundle generates for a\n    deployed skill (info.title \"Kana API\"; components.securitySchemes.apikey =\n    {type: apiKey, in: header, name: x-kana-apikey}; every operation carries\n    security: [{apikey: []}] and a documented 401 \"Invalid apikey specified\").\n    The generated document is rendered in a Swagger UI inside the signed-in console;\n    it is not published at a public URL, so no spec was saved to openapi/.\n  evidence:\n    url: https://apps.kana.ai/index.js\n    http_status: 200\n    fetched: '2026-08-13'\ngated: true\ngate_note: >-\n  API keys are issued from the signed-in Kana console (apps.kana.ai); there is no\n  public developer portal, no anonymous key issuance, and no public auth documentation\n  page. Every apps.kana.ai path except the OAuth metadata answers 401.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kana/refs/heads/main/authentication/kana-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Marketing
- Artificial Intelligence
- Agentic AI
- Marketing Technology
- Audience Intelligence
- Customer Data Platform
- AI Search Optimization
- Growth
---
