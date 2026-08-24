---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Hypernative Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hypernative declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hypernative
provider_slug: hypernative
scheme_count: 2
schemes:
- confidence: high
  evidence: 'Public Balancer integration code sends `Authorization: Bearer ${apiKey}` to https://api.hypernative.xyz/assets/reputation/addresses. An unauthenticated POST to that exact endpoint returned HTTP 401 with {"success":false,"error":"Unauthorized","errorCode":401} on 2026-08-22, confirming the endpoint exists and is credential-gated.'
  format: Bearer <apiKey>
  header: Authorization
  in: header
  key: bearerAuth
  scheme: bearer
  type: http
- confidence: low
  evidence: Hypernative's app issues client-id / client-secret pairs for programmatic access per its login surface, but the header names could NOT be confirmed from any public document — the API reference is gated. Recorded as a low-confidence candidate ONLY; do not treat these header names as verified.
  headers:
  - x-client-id
  - x-client-secret
  in: header
  key: clientCredentials
  type: apiKey
slug: hypernative-authentication
source_filename: hypernative-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of https://api.hypernative.xyz (2026-08-22) plus public\n  third-party integration source code that calls the Hypernative API\n  (https://github.com/balancer/balancer-api/blob/master/src/lambdas/check-wallet.ts).\n  The provider's own auth reference is inside the authenticated GitBook space at\n  docs.hypernative.xyz and could not be read.\napi: Hypernative API\nbase_url: https://api.hypernative.xyz\nschemes:\n- key: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <apiKey>'\n  confidence: high\n  evidence: >-\n    Public Balancer integration code sends\n    `Authorization: Bearer ${apiKey}` to\n    https://api.hypernative.xyz/assets/reputation/addresses. An unauthenticated POST to\n    that exact endpoint returned HTTP 401 with\n    {\"success\":false,\"error\":\"Unauthorized\",\"errorCode\":401} on 2026-08-22, confirming the\n    endpoint\
  \ exists and is credential-gated.\n- key: clientCredentials\n  type: apiKey\n  in: header\n  headers:\n  - x-client-id\n  - x-client-secret\n  confidence: low\n  evidence: >-\n    Hypernative's app issues client-id / client-secret pairs for programmatic access\n    per its login surface, but the header names could NOT be confirmed from any public\n    document — the API reference is gated. Recorded as a low-confidence candidate ONLY;\n    do not treat these header names as verified.\noauth2: false\nopenid_connect: false\nmutual_tls: unknown\nscopes:\n  published: false\n  note: >-\n    No OAuth2 scope surface. Access appears to be bearer-token/API-key based, so\n    scopes/ is not applicable (see the key-auth guidance in the pipeline contract).\n    Role/permission granularity, if any, is documented only inside the gated docs.\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  note: All OAuth/OIDC discovery documents 404 on every\
  \ Hypernative host.\nobserved_challenge:\n  request: POST https://api.hypernative.xyz/assets/reputation/addresses (no credentials)\n  status: 401\n  www_authenticate: null\n  body: '{\"success\":false,\"data\":{},\"error\":\"Unauthorized\",\"errorCode\":401,\"version\":\"2.59.0+3f613ebbd\",\"service\":\"@hypernative/server\"}'\n  note: >-\n    No WWW-Authenticate header is returned on the 401, so the required scheme is not\n    machine-discoverable from the challenge — a client must read the gated docs.\ntransport_security:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: 'max-age=15552000; includeSubDomains'\n  observed_headers:\n  - content-security-policy\n  - cross-origin-opener-policy: same-origin\n  - cross-origin-resource-policy: same-origin\n  - referrer-policy: no-referrer\n  - x-content-type-options: nosniff\n  - x-frame-options: SAMEORIGIN\n  note: >-\n    The API sends a full Helmet-style hardening header set on every response including\n    error responses.\ndocs: https://docs.hypernative.xyz/\n\
  docs_accessible: false\ndocs_note: >-\n  docs.hypernative.xyz 307-redirects every path to\n  https://app.hypernative.xyz/login?ref=gitbook — the entire API reference is a\n  customer-only GitBook space.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypernative/refs/heads/main/authentication/hypernative-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- Blockchain
- Web3
- Threat Detection
- Risk Management
- Compliance
- Fraud Prevention
- Monitoring
- Cryptocurrency
---
