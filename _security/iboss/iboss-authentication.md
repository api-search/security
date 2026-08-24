---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Iboss Authentication
name_suffix: Authentication
oauth_flows: []
overview: iboss declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: iboss
provider_slug: iboss
scheme_count: 2
schemes:
- confidence: high
  evidence: Set-Cookie observed on anonymous 401 from /ibcloud/web/users
  id: session-cookie
  in: cookie
  mechanism: session
  name: JSESSIONID
  type: http
- confidence: high
  evidence: Set-Cookie observed on anonymous 401 from /ibcloud/web/users
  id: xsrf-token
  in: cookie
  mechanism: csrf-double-submit
  name: XSRF-TOKEN
  note: A CSRF defence, not an authorization credential. Recorded because it is a required part of any successful state-changing call against this surface.
  type: apiKey
slug: iboss-authentication
source_filename: iboss-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://api.ibosscloud.com/ibcloud/web/users\nnote: >-\n  DERIVED FROM LIVE PROBE RESPONSE HEADERS ONLY. iboss publishes no OpenAPI definition\n  and no public authentication documentation, so no securityScheme could be read from a\n  contract. Everything below was observed on an anonymous request and nothing has been\n  inferred beyond what the response actually returned. The scheme names used by the\n  platform's own login flow are NOT published and are therefore not asserted here.\nsurface:\n  base_url: https://api.ibosscloud.com/ibcloud/web\n  alternate_hosts:\n  - https://cloud.iboss.com/ibcloud/web\n  auth_host: https://accounts.iboss.com/ibossauth/index.html\n  public_documentation: false\nobserved:\n  anonymous_request:\n    method: GET\n    path: /ibcloud/web/users\n    status: 401\n    server_header: iboss cloud\n    content_length: 0\n    www_authenticate: null\n    note: >-\n      Returns a bare 401 with no WWW-Authenticate\
  \ challenge and an empty body, so the\n      API does not advertise its scheme to an unauthenticated caller. An agent cannot\n      discover how to authenticate from the response.\n  cookies_issued:\n  - name: XSRF-TOKEN\n    path: /ibcloud\n    attributes: [Secure]\n    http_only: false\n    purpose: >-\n      Double-submit CSRF token. Readable by JavaScript by design so the console can echo\n      it in a request header — the classic Spring Security XSRF pattern.\n  - name: JSESSIONID\n    path: /ibcloud\n    attributes: [Secure, HttpOnly]\n    http_only: true\n    purpose: Server-side session identifier for the authenticated console session.\n  security_headers:\n    strict_transport_security: max-age=63072000; includeSubDomains\n    x_frame_options: DENY\n    x_content_type_options: nosniff\n    x_xss_protection: 1; mode=block\n    x_robots_tag: noindex, nofollow\n    cache_control: no-cache, no-store, max-age=0, must-revalidate\nschemes:\n- id: session-cookie\n  type: http\n  mechanism:\
  \ session\n  in: cookie\n  name: JSESSIONID\n  evidence: Set-Cookie observed on anonymous 401 from /ibcloud/web/users\n  confidence: high\n- id: xsrf-token\n  type: apiKey\n  mechanism: csrf-double-submit\n  in: cookie\n  name: XSRF-TOKEN\n  evidence: Set-Cookie observed on anonymous 401 from /ibcloud/web/users\n  confidence: high\n  note: >-\n    A CSRF defence, not an authorization credential. Recorded because it is a required\n    part of any successful state-changing call against this surface.\noauth2: false\napi_keys:\n  published: false\n  note: >-\n    No public documentation of an API key or token issuance flow was found on any iboss\n    host, in the sitemap (344 URLs, no /api or /developer route), or in llms.txt.\nmutual_tls: false\ngaps:\n- No public authentication documentation page.\n- No WWW-Authenticate header on 401, so the scheme is not machine-discoverable.\n- No OpenAPI securitySchemes block, because no OpenAPI is published.\n- No OAuth 2.0 or OIDC discovery document\
  \ on any host (see well-known/iboss-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iboss/refs/heads/main/authentication/iboss-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Zero Trust
- SASE
- Secure Web Gateway
- CASB
- ZTNA
- Data Loss Prevention
- Network Security
- Cloud Security
- Compliance
---
