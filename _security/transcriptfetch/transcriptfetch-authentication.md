---
anonymous_access: false
api_key_in: []
api_specs:
- filename: transcriptfetch-api-v2-openapi.json
  format: json
  label: TranscriptFetch REST API
  slug: transcriptfetch-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/openapi/transcriptfetch-api-v2-openapi.json
auth_types:
- http
- oauth2 (MCP surface)
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Transcriptfetch Authentication
name_suffix: Authentication
oauth_flows: []
overview: TranscriptFetch secures its APIs with http and oauth2 (MCP surface) across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TranscriptFetch
provider_slug: transcriptfetch
scheme_count: 2
schemes:
- description: 'Send your API key as `Authorization: Bearer <key>`.'
  key_prefix: tf_live_
  name: bearerAuth
  notes:
  - Keys are created in the dashboard; a SHA-256 hash is stored server-side, never the plaintext, so a key cannot be shown again after creation.
  - Multiple keys per account, independently revocable (immediate), each with its own rate limit — rotation without downtime.
  - Send keys only in the Authorization header, never a query string or browser JavaScript; the API deliberately sends no CORS headers.
  scheme: bearer
  sources:
  - openapi/transcriptfetch-api-v1-openapi.json
  - openapi/transcriptfetch-api-v2-openapi.json
  type: http
- description: OAuth 2.0 authorization-code with PKCE (S256) against the Clerk-run authorization server at clerk.transcriptfetch.com, with dynamic client registration. RFC 9728 protected-resource metadata at /.well-known/oauth-protected-resource names the MCP endpoint as the resource. The MCP server also accepts the same tf_live_ bearer keys.
  metadata:
  - well-known/transcriptfetch-oauth-protected-resource.json
  - well-known/clerk-transcriptfetch-oauth-authorization-server.json
  name: mcp-oauth
  surface: MCP server only (https://transcriptfetch.com/mcp)
  type: oauth2
slug: transcriptfetch-authentication
source_filename: transcriptfetch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: openapi/transcriptfetch-api-v1-openapi.json, openapi/transcriptfetch-api-v2-openapi.json\ndocs: https://transcriptfetch.com/docs/api-reference\nsummary:\n  types:\n  - http\n  - oauth2 (MCP surface)\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Send your API key as `Authorization: Bearer <key>`.'\n  key_prefix: tf_live_\n  sources:\n  - openapi/transcriptfetch-api-v1-openapi.json\n  - openapi/transcriptfetch-api-v2-openapi.json\n  notes:\n  - Keys are created in the dashboard; a SHA-256 hash is stored server-side, never the plaintext, so a key cannot be shown again after creation.\n  - Multiple keys per account, independently revocable (immediate), each with its own rate limit — rotation without downtime.\n  - Send keys only in the Authorization header, never a query string or browser JavaScript; the API deliberately sends no CORS headers.\n- name: mcp-oauth\n  type: oauth2\n  surface: MCP server\
  \ only (https://transcriptfetch.com/mcp)\n  description: >-\n    OAuth 2.0 authorization-code with PKCE (S256) against the Clerk-run authorization\n    server at clerk.transcriptfetch.com, with dynamic client registration. RFC 9728\n    protected-resource metadata at /.well-known/oauth-protected-resource names the MCP\n    endpoint as the resource. The MCP server also accepts the same tf_live_ bearer keys.\n  metadata:\n  - well-known/transcriptfetch-oauth-protected-resource.json\n  - well-known/clerk-transcriptfetch-oauth-authorization-server.json\npublic_endpoints:\n- GET /api/v2/health and /api/v2/health/deep need no key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/authentication/transcriptfetch-authentication.yml
summary_line: http/oauth2 (MCP surface) · 2 schemes
tags:
- transcripts
- speech-to-text
- captions
- youtube
- tiktok
- instagram
- podcasts
- mcp
- llms-txt
- openapi
- Transcription
- Speech-to-Text
- Video
- Podcasts
- AI/LLM
- RAG
- Agents
- MCP
- Developer Tools
- Media
- Content
- YouTube
- TikTok
- Instagram
- Spotify
- Apple Podcasts
---
