---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Bianhuakai Club Authentication
name_suffix: Authentication
oauth_flows: []
overview: OPC / 彼岸花开 declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: OPC / 彼岸花开
provider_slug: bianhuakai-club
scheme_count: 0
schemes: []
slug: bianhuakai-club-authentication
source_filename: bianhuakai-club-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: securitySchemes on https://bianhuakai.club/.well-known/agent.json + an anonymous POST to https://bianhuakai.club/a2a/, 2026-09-19\nsummary: >-\n  The A2A JSON-RPC endpoint is anonymous. The agent card declares securitySchemes {} and no\n  security[] requirement, and a POST with no Authorization header was answered with a JSON-RPC\n  envelope (HTTP 200), so no credential of any kind gates the agent surface. The consumer chat app\n  at the site root and the \"Chat with me\" widget on /lei/ use an email + verification-code login\n  (client-side calls to /auth/register, /auth/verify, /auth/login, /auth/forgot, /auth/reset) - a\n  human account system for the web UI, not a developer credential, and not documented as an API.\n  There is no OAuth, no OIDC discovery, no API keys and no developer signup.\nschemes: []\nscheme_count: 0\nagent_surface:\n  endpoint: https://bianhuakai.club/a2a/\n  auth: none\n  evidence: \"card securitySchemes\
  \ is {}; anonymous POST answered 200 with a JSON-RPC error envelope (-32601 for an unknown method)\"\n  cors_allowed_headers: [Content-Type, Authorization, x-broker-token]\n  cors_note: \"the CORS allow-list names Authorization and x-broker-token, so the server is prepared to receive them, but nothing published requires either\"\noauth: false\nopenid_configuration_status: 404\noauth_authorization_server_status: 404\noauth_protected_resource_status: 404\ndocs: null\ndocs_note: no authentication documentation is published\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bianhuakai-club/refs/heads/main/authentication/bianhuakai-club-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Agents
- A2A
- Video
- Video Production
- China
- Hangzhou
- Travel
- Genealogy
- Real-Estate
- Documentary
- Local Services
- One-Person Company
---
