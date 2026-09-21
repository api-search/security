---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Perkoon Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perkoon declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Perkoon
provider_slug: perkoon-com
scheme_count: 4
schemes:
- applies_to:
    a2a:
    - POST /a2a (describe
    - send-files
    - receive-files
    - session-status)
    cli:
    - perkoon send
    - perkoon receive
    mcp:
    - send_file
    - receive_file
    - check_session
    rest:
    - POST /api/v1/sessions
    - POST /api/v1/sessions/{code}/join
    - GET /api/v1/sessions/{code}/status
  detail: No Authorization header, API key, cookie or account is required or documented. Rate limiting keys on IP (see rate-limits/).
  id: none
  observed:
  - method: GET
    note: no securitySchemes / security field in the card
    status: 200
    url: https://perkoon.com/.well-known/agent-card.json
  - note: called by @perkoon/mcp with a bare fetch() and no headers (src/index.js); not probed live - robots.txt disallows /api/
    url: https://perkoon.com/api/v1/sessions/{code}/status
  type: none
- applies_to:
    cli:
    - send --password <pw>
    - receive --password <pw>
    mcp:
    - send_file.password
    - receive_file.password
  detail: 'Optional; set by the sender, required by the receiver to join. Max 512 characters (MCP zod schema). Wrong password -> CLI exit code 4 (Auth error). SKILL.md: "For sensitive files, always use --password — without it, anyone with the share link can download."'
  id: session-password
  type: shared-secret (per session)
- applies_to:
    a2a:
    - send-files response
    cli:
    - send <file> --session <code> --sender-key <key>
  detail: Returned to whoever creates a session over A2A; lets a CLI process attach as the sender of that session. Not an account credential.
  id: sender-key
  type: capability token (per session)
- applies_to:
    browser:
    - POST /create
  detail: 'Phoenix protect_from_forgery: session cookie + _csrf_token (from <meta name="csrf-token">) required; missing -> 403 InvalidCSRFTokenError. llms.txt directs cookie-less agents to POST /a2a instead.'
  id: csrf-browser-pipeline
  type: anti-forgery (not authentication)
slug: perkoon-com-authentication
source_filename: perkoon-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://perkoon.com/llms.txt\nsource: >-\n  https://perkoon.com/llms.txt, https://perkoon.com/.well-known/agent-card.json, the perkoon 0.5.7 README (--password,\n  --session, --sender-key), the @perkoon/mcp 0.3.0 source (anonymous fetch of /api/v1/sessions/{code}/status), and the\n  /.well-known/ probe in well-known/perkoon-com-well-known.yml - all 2026-09-19. derive-authentication.py was not run:\n  there is no OpenAPI to derive from.\nsummary: >-\n  Every machine surface Perkoon publishes is anonymous and account-less (\"No accounts\" - llms.txt and the agent card).\n  There is no API key, no OAuth authorization server, no OpenID configuration, no protected-resource metadata, no\n  dynamic client registration and no developer sign-up; the A2A card declares no securitySchemes. Access control is\n  per session, not per caller: an optional password set by the sender (CLI --password, MCP password, wrong password ->\n  CLI exit\
  \ 4), and a sender-key that the A2A send-files skill returns to the session creator so a CLI process can\n  attach as sender (--session <code> --sender-key <key>). The browser entry point /create is the one exception in\n  mechanism, not in identity: it requires a Phoenix session cookie plus a _csrf_token read from a prior page load\n  (without it, 403 InvalidCSRFTokenError), which is anti-forgery, not authentication. The site's edge adds a\n  Cloudflare managed challenge on HTML routes and on /a2a for non-browser clients, which is a bot policy rather than\n  an auth scheme, recorded here because it is what an agent actually meets first.\nschemes:\n- id: none\n  type: none\n  applies_to:\n    rest: [POST /api/v1/sessions, 'POST /api/v1/sessions/{code}/join', 'GET /api/v1/sessions/{code}/status']\n    a2a: [POST /a2a (describe, send-files, receive-files, session-status)]\n    mcp: [send_file, receive_file, check_session]\n    cli: [perkoon send, perkoon receive]\n  detail: No Authorization\
  \ header, API key, cookie or account is required or documented. Rate limiting keys on IP (see rate-limits/).\n  observed:\n  - {url: https://perkoon.com/.well-known/agent-card.json, method: GET, status: 200, note: no securitySchemes / security field in the card}\n  - {url: 'https://perkoon.com/api/v1/sessions/{code}/status', note: 'called by @perkoon/mcp with a bare fetch() and no headers (src/index.js); not probed live - robots.txt disallows /api/'}\n- id: session-password\n  type: shared-secret (per session)\n  applies_to:\n    cli: ['send --password <pw>', 'receive --password <pw>']\n    mcp: [send_file.password, receive_file.password]\n  detail: 'Optional; set by the sender, required by the receiver to join. Max 512 characters (MCP zod schema). Wrong password -> CLI exit code 4 (Auth error). SKILL.md: \"For sensitive files, always use --password — without it, anyone with the share link can download.\"'\n- id: sender-key\n  type: capability token (per session)\n  applies_to:\n    cli:\
  \ ['send <file> --session <code> --sender-key <key>']\n    a2a: ['send-files response']\n  detail: Returned to whoever creates a session over A2A; lets a CLI process attach as the sender of that session. Not an account credential.\n- id: csrf-browser-pipeline\n  type: anti-forgery (not authentication)\n  applies_to:\n    browser: ['POST /create']\n  detail: 'Phoenix protect_from_forgery: session cookie + _csrf_token (from <meta name=\"csrf-token\">) required; missing -> 403 InvalidCSRFTokenError. llms.txt directs cookie-less agents to POST /a2a instead.'\noauth:\n  authorization_server_metadata: {url: https://perkoon.com/.well-known/oauth-authorization-server, status: 404}\n  protected_resource_metadata: {url: https://perkoon.com/.well-known/oauth-protected-resource, status: 404}\n  openid_configuration: {url: https://perkoon.com/.well-known/openid-configuration, status: 404}\n  dynamic_client_registration: false\n  scopes: none - no scopes artifact is written because no OAuth surface\
  \ exists\ntransport_security:\n  tls: TLSv1.3, HSTS max-age=31536000; includeSubDomains; preload (security/perkoon-com-domain-security.yml)\n  p2p: 'WebRTC data channels (DTLS-encrypted per SKILL.md); perkoon.com performs signalling only and \"your data never touches our servers\" for P2P (README)'\nedge_policy:\n  note: 'Cloudflare managed challenge (HTTP 403, cf-mitigated: challenge) on every HTML route and on POST /a2a for curl with or without a browser User-Agent on 2026-09-19; /.well-known/agent-card.json, /.well-known/agent.json, /llms.txt and /robots.txt are exempt. Not evaded.'\ngated_surfaces:\n  note: robots.txt disallows /api/, /analytics/ and /gx7k9m2p5/ (admin). The /api/ disallow covers the REST session paths the CLI uses; they were not probed live in deference to it, and everything recorded about them is transcribed from the provider's own packages and llms.txt.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perkoon-com/refs/heads/main/authentication/perkoon-com-authentication.yml
summary_line: 4 schemes
tags:
- File Transfer
- P2P
- WebRTC
- AI Agents
- A2A
- MCP
- CLI
- Agent Skills
- Cloud Storage
- Developer Tools
- Lithuania
---
