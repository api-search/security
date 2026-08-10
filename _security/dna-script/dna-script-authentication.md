---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Dna Script Authentication
name_suffix: Authentication
oauth_flows: []
overview: DNA Script declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: DNA Script
provider_slug: dna-script
scheme_count: 0
schemes: []
slug: dna-script-authentication
source_filename: dna-script-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://syntax.dnascript.com/graphql\ndocs: null\nsummary:\n  types: []\n  documented_publicly: false\n  note: >-\n    DNA Script publishes NO public authentication documentation, no developer\n    portal and no machine-readable security scheme. This profile is what was\n    observed on the wire, not what the provider documents. It is deliberately NOT\n    wired as a canonical `Authentication` pointer in apis.yml, because the\n    ergonomics check that pointer feeds is \"authentication documented\" — and it is\n    not.\nobserved:\n- surface: https://syntax.dnascript.com/graphql\n  transport: HTTPS POST (GraphQL over HTTP)\n  anonymous_introspection: true\n  anonymous_operations: false\n  unauthenticated_response:\n    http_status: 401\n    content_type: application/json;charset=UTF-8\n    body_shape: '{\"timestamp\":\"...\",\"status\":401,\"error\":\"Unauthorized\",\"path\":\"/graphql\"}'\n  inferred_model: >-\n    Customer\
  \ session established through the SYNTAX Console web application at\n    https://syntax.dnascript.com/. The schema exposes login/logout, password\n    reset, email confirmation, invitation and \"loginAs\" mutations, plus a role and\n    group model (AccessPermission = WRITE | ADMIN | SERVICE) — i.e. an\n    organization-scoped, role-based product login, not an API-key or OAuth\n    developer credential.\n  schema_evidence:\n    mutations:\n    - logout\n    - changePassword\n    - changePasswordForUser\n    - forgotPassword\n    - resetPassword\n    - setPasswordForInvitedUser\n    - confirmEmail\n    - resendEmailActivation\n    - inviteUser\n    - loginAs\n    - deleteSessions\n    queries:\n    - getCurrentUser\n    - getAllRoles\n    - getLoginEvents\n    - validateVerificationCode\n    enums:\n      AccessPermission:\n      - WRITE\n      - ADMIN\n      - SERVICE\n- surface: https://syntax.dnascript.com/api/*\n  note: >-\n    Every REST path under /api (including /api/openapi.json,\
  \ /api/v3/api-docs,\n    /api/swagger-ui/index.html, /api/actuator/health) returns 401 Unauthorized\n    with the same Spring-style JSON envelope. No spec is served anonymously.\nnot_found:\n- oauth2 authorization server metadata (RFC 8414)\n- OpenID Connect discovery document\n- API keys / personal access tokens (no public issuance surface)\n- mTLS or signed-request scheme\n- any published auth guide, quickstart, or developer terms\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - url: https://syntax.dnascript.com/graphql\n    method: POST\n    http_status: 200\n    note: introspection query only; no data query was issued\n  - url: https://syntax.dnascript.com/graphql\n    method: GET\n    http_status: 401\n  - url: https://syntax.dnascript.com/api/openapi.json\n    http_status: 401\n  - url: https://syntax.dnascript.com/api/v3/api-docs\n    http_status: 401\n  - url: https://syntax.dnascript.com/api/.well-known/openid-configuration\n    http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dna-script/refs/heads/main/authentication/dna-script-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Synthetic Biology
- Life Sciences
- DNA Synthesis
- Laboratory Instruments
- Genomics
- Scientific Computing
- GraphQL
---
