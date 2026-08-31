---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Tailor Brands Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tailor Brands declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tailor Brands
provider_slug: tailor-brands
scheme_count: 2
schemes:
- confidence: medium
  evidence: 401 body "missing authentication header (Authorization or X-API-Key required)" names Authorization as an accepted header; the token format is not published.
  id: bearer-authorization
  in: header
  name: Authorization
  scheme: bearer
  type: http
- confidence: medium
  evidence: 401 body names X-API-Key as the alternative accepted header; key format, prefix and issuance flow are not published.
  id: api-key
  in: header
  name: X-API-Key
  type: apiKey
slug: tailor-brands-authentication
source_filename: tailor-brands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  live HTTP probes of https://api.tailorbrands.com/v1/* (2026-08-29); no OpenAPI\n  securitySchemes exist to derive from and no public auth documentation was found\nnote: >-\n  This profile is PROBED, not derived. Tailor Brands publishes no OpenAPI and no public\n  authentication documentation, but the live API host states its own requirement in the\n  401 response body. Every path under /v1/ — including a deliberately nonexistent control\n  path — returns the identical plain-text response, so the gate is applied at the edge\n  across the whole namespace rather than per-operation. The response carries no\n  WWW-Authenticate header, no OAuth challenge and no link to documentation, so an\n  integrator cannot discover the token format, header syntax or issuance flow without a\n  partner conversation.\nschemes:\n- id: bearer-authorization\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  confidence: medium\n\
  \  evidence: >-\n    401 body \"missing authentication header (Authorization or X-API-Key required)\" names\n    Authorization as an accepted header; the token format is not published.\n- id: api-key\n  type: apiKey\n  in: header\n  name: X-API-Key\n  confidence: medium\n  evidence: >-\n    401 body names X-API-Key as the alternative accepted header; key format, prefix and\n    issuance flow are not published.\noauth2: false\nopenid_connect: false\nmutual_tls: unknown\nkey_issuance: >-\n  Not public. Access to the Tailor Embedded API is granted through the partner early-access\n  program at https://www.tailorbrands.com/embedded.\ndocs: null\ndocs_note: No public authentication reference page was found on any Tailor Brands host.\nx-evidence:\n- url: https://api.tailorbrands.com/v1/openapi.json\n  http_status: 401\n  body: 'missing authentication header (Authorization or X-API-Key required)'\n- url: https://api.tailorbrands.com/v1/businesses\n  http_status: 401\n  body: 'missing authentication\
  \ header (Authorization or X-API-Key required)'\n- url: https://api.tailorbrands.com/v1/zzz-nonexistent-path-xyz\n  http_status: 401\n  body: 'missing authentication header (Authorization or X-API-Key required)'\n  finding: >-\n    control probe — a path that cannot exist returns the same 401, proving the gate is\n    namespace-wide and that the 401 at /v1/openapi.json is NOT evidence a spec is served there\n- url: https://api.tailorbrands.com/\n  http_status: 404\n  body: '404 page not found'\n  finding: outside /v1/ the host 404s in plain text, so the 401 is auth, not a catch-all\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailor-brands/refs/heads/main/authentication/tailor-brands-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Business Formation
- Compliance
- Small Business
- Branding
- Legal
- Registered Agent
- Embedded Finance
- Artificial Intelligence
- Logo Design
---
