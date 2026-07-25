---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Ebix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ebix declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Ebix
provider_slug: ebix
scheme_count: 0
schemes: []
slug: ebix-authentication
source_filename: ebix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: >-\n  Live probes of api.ebixcash.com, api.ebix.com, ebixcash.com and ebixasp.com;\n  EbixASP product help. No OpenAPI exists in this repo to derive from\n  (derive-authentication.py has no input).\ndocumented: false\nnote: >-\n  Ebix publishes NO public authentication documentation. This file records what\n  was observed on the wire, not a documented contract — no `Authentication`\n  pointer is wired into apis.yml, because the check it feeds asks whether\n  authentication is documented, and it is not.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  discovery:\n    openid_configuration: 404\n    oauth_authorization_server: 404\nschemes: []\nobserved:\n- host: https://api.ebixcash.com\n  surface: EbixCash API Hub (uvicorn / FastAPI)\n  evidence: >-\n    GET /openapi.json -> HTTP 401 {\"detail\":\"Missing Authorization header\"}.\n    An Authorization header is required; the scheme (Bearer/JWT/API key/Basic)\n \
  \   is not disclosed by the challenge and no WWW-Authenticate header is\n    returned.\n  scheme: undisclosed\n- host: https://api.ebix.com\n  surface: gateway\n  evidence: >-\n    GET / and every probed path -> HTTP 404\n    { \"statusCode\": 404, \"message\": \"Resource not found\" }. No authentication\n    challenge is reachable because no route is publicly addressable.\n  scheme: unknown\n- host: https://ebixcash.com/api/\n  surface: edge/WAF JSON envelope\n  evidence: >-\n    GET -> 405 {\"status\":405,\"uri\":\"/api/\",\"reference\":\"...\"}; POST -> 400\n    {\"status\":400,...}. A generic edge error envelope with a request reference\n    id, not a documented API surface.\n  scheme: unknown\n- host: https://www.ebixasp.com\n  surface: EbixASP agency application + support portal\n  evidence: >-\n    /support serves an HTML username/password form posting to\n    /support/index.asp (\"Currently no session is active. Please login.\"). Agency\n    access is session-based web login, not\
  \ a token-based API auth model.\n  scheme: form-login (session)\n- host: IVANS\n  surface: EbixASP Real-Time Interface\n  evidence: >-\n    \"When logging onto the EbixASP Real Time Interface the PC synchronizes with\n    IVANS and updates the credentials on the PC, including the list of carriers\n    and service transactions IVANS has set up for the agency's account.\" Carrier\n    download credentials are provisioned through IVANS, out of band.\n  scheme: provisioned-credentials (out-of-band)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebix/refs/heads/main/authentication/ebix-authentication.yml
summary_line: 0 schemes
tags:
- Insurance
- United States
- Property and Casualty
- Life Insurance
- Health Insurance
- Employee Benefits
- Agency Management
- Policy Administration
- Claims
- ACORD
- Insurtech
- Market Infrastructure
---
