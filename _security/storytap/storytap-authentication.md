---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Storytap Authentication
name_suffix: Authentication
oauth_flows: []
overview: StoryTap declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: StoryTap
provider_slug: storytap
scheme_count: 2
schemes:
- aliases:
  - key
  applies_to:
  - POST https://api.storytap.com/w/get-embed
  - POST https://api.storytap.com/w/answer
  - POST https://api.storytap.com/w/question
  - POST https://api.storytap.com/w/v-feedback
  - POST https://api.storytap.com/w/event-queue
  companion_parameters:
  - meaning: embed id — identifies which embed/brand the request is for
    name: eid
  - meaning: optional store scope
    name: storeId
  - added by the loader: null
    meaning: window.location.hostname
    name: origin
  - added by the loader: null
    meaning: full page URL
    name: source
  id: embed-public-key
  in: body
  name: k
  note: 'The key is published in the host page''s embed markup, so any site visitor can read it. It scopes a request to a brand''s embed rather than authenticating a principal. CORS is fully open (access-control-allow-origin: *), so the practical control is the origin/source values the loader supplies, which a caller can set freely. Treat this as identification, not authentication.'
  secrecy: public
  type: apiKey
- applies_to: StoryTap Enterprise REST API (campaigns, brands, invites, events)
  evidence: Existence is established by StoryTap's own Zapier app, StoryTapCLIAPI@1.6.1 (https://zapier.com/apps/storytap/integrations), which necessarily authenticates to a StoryTap account. The listing does not disclose the auth type, and StoryTap publishes no auth documentation, so nothing further is asserted here.
  id: enterprise-platform-api
  in: unknown
  type: unknown
slug: storytap-authentication
source_filename: storytap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  Request construction read from StoryTap's public embed loader\n  https://cdn1aws.storytap.com/storytap-videos-2.js and confirmed against live\n  responses from https://api.storytap.com/w/*. derive-authentication.py produced\n  nothing because StoryTap publishes no OpenAPI to derive securitySchemes from.\ndocs: null\ndocs_note: StoryTap publishes no authentication documentation on any host.\nsummary: >-\n  The only StoryTap API surface reachable without credentials authenticates with\n  a PUBLIC per-embed key carried in the JSON request body — not a header, not a\n  bearer token, and not a secret. The authenticated Enterprise platform API has\n  no publicly documented authentication scheme at all.\nschemes:\n  - id: embed-public-key\n    type: apiKey\n    in: body\n    name: k\n    aliases: [key]\n    companion_parameters:\n      - {name: eid, meaning: embed id — identifies which embed/brand the request is for}\n      -\
  \ {name: storeId, meaning: optional store scope}\n      - {name: origin, meaning: window.location.hostname, added by the loader}\n      - {name: source, meaning: full page URL, added by the loader}\n    applies_to:\n      - POST https://api.storytap.com/w/get-embed\n      - POST https://api.storytap.com/w/answer\n      - POST https://api.storytap.com/w/question\n      - POST https://api.storytap.com/w/v-feedback\n      - POST https://api.storytap.com/w/event-queue\n    secrecy: public\n    note: >-\n      The key is published in the host page's embed markup, so any site visitor\n      can read it. It scopes a request to a brand's embed rather than\n      authenticating a principal. CORS is fully open\n      (access-control-allow-origin: *), so the practical control is the\n      origin/source values the loader supplies, which a caller can set freely.\n      Treat this as identification, not authentication.\n  - id: enterprise-platform-api\n    type: unknown\n    in: unknown\n    applies_to:\
  \ 'StoryTap Enterprise REST API (campaigns, brands, invites, events)'\n    evidence: >-\n      Existence is established by StoryTap's own Zapier app,\n      StoryTapCLIAPI@1.6.1 (https://zapier.com/apps/storytap/integrations), which\n      necessarily authenticates to a StoryTap account. The listing does not\n      disclose the auth type, and StoryTap publishes no auth documentation, so\n      nothing further is asserted here.\nnegative_findings:\n  - {check: OAuth 2.0 authorization server metadata, url: 'https://api.storytap.com/.well-known/oauth-authorization-server', status: 404}\n  - {check: OAuth 2.0 protected resource metadata, url: 'https://api.storytap.com/.well-known/oauth-protected-resource', status: 404}\n  - {check: OpenID Connect discovery, url: 'https://app.storytap.com/.well-known/openid-configuration', status: 404}\n  - {check: Authorization header accepted, result: 'not used by the client and not required by the server'}\n  - {check: mTLS, result: not offered}\noauth_scopes:\
  \ none\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n    - {url: 'https://api.storytap.com/w/get-embed', method: POST, status: 200, body: '{\"error\":\"Missing required data\"}'}\n    - {url: 'https://api.storytap.com/w/get-embed', method: OPTIONS, status: 200, note: 'access-control-allow-origin: *; allow-methods GET,POST'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storytap/refs/heads/main/authentication/storytap-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Video
- Testimonials
- User Generated Content
- Marketing
- Reviews
- Video Testimonials
- SaaS
---
