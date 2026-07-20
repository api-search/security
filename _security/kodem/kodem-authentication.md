---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Kodem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kodem secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kodem
provider_slug: kodem
scheme_count: 2
schemes:
- confidence: probed
  evidence: 'Advertised in the CORS access-control-allow-headers of the API host response: content-type, authorization, x-kodem-apikey, user-agent, dnt, sec-ch-ua, sec-ch-ua-mobile, sec-ch-ua-platform.'
  in: header
  name: x-kodem-apikey
  parameter_name: x-kodem-apikey
  type: apiKey
- confidence: probed
  evidence: The authorization header is also advertised in access-control-allow-headers, but the scheme (bearer/basic) is not observable without a credential and is not documented publicly.
  name: authorization
  scheme: unknown
  type: http
slug: kodem-authentication
source_filename: kodem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live HTTP probes of https://api.kodemsecurity.com (no OpenAPI is published, so no securitySchemes\n  could be derived)\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  fully_gated: true\nschemes:\n- name: x-kodem-apikey\n  type: apiKey\n  in: header\n  parameter_name: x-kodem-apikey\n  confidence: probed\n  evidence: 'Advertised in the CORS access-control-allow-headers of the API host response: content-type,\n    authorization, x-kodem-apikey, user-agent, dnt, sec-ch-ua, sec-ch-ua-mobile, sec-ch-ua-platform.'\n- name: authorization\n  type: http\n  scheme: unknown\n  confidence: probed\n  evidence: 'The authorization header is also advertised in access-control-allow-headers, but the scheme\n    (bearer/basic) is not observable without a credential and is not documented publicly.'\nposture:\n  unauthenticated_status: 401\n  unauthenticated_body: '{\"detail\":\"Unauthorized\"}'\n  paths_probed:\
  \ 17\n  paths_reachable_unauthenticated: 0\n  allowed_methods:\n  - GET\n  - POST\n  - PUT\n  - DELETE\n  - OPTIONS\n  allow_credentials: true\n  notes: 'Every path probed on api.kodemsecurity.com — including /, /openapi.json, /swagger.json, /docs,\n    /redoc, /health, /v1 and /.well-known/* — returns 401 with the same JSON envelope. The API is real\n    and actively served but entirely closed to unauthenticated discovery; no public reference, OpenAPI\n    document, or auth guide is published. Product documentation sits behind the application login at\n    docs.kodemsecurity.com, which redirects unauthenticated visitors to app.kodemsecurity.com.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kodem/refs/heads/main/authentication/kodem-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Cybersecurity
- Application Security
- Runtime Security
- Software Composition Analysis
- Static Analysis
- Vulnerability Management
- DevSecOps
- SBOM
- AI Security
---
