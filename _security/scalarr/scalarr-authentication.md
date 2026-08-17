---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Scalarr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalarr declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Scalarr
provider_slug: scalarr
scheme_count: 0
schemes: []
slug: scalarr-authentication
source_filename: scalarr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://github.com/agent-defense/parallax (README, docs/integrations/generic.md,\n  src/server/api.rs), a live unauthenticated probe of https://portal.edgelabs.ai/api/,\n  and the identity providers referenced in the portal application bundle\n  https://portal.edgelabs.ai/main.f9a8cb7963b57ff8.js\nnote: >-\n  Scalarr publishes no OpenAPI, so there are no securitySchemes to derive from;\n  this profile is built from the provider's own source/docs and from what the\n  live endpoints actually returned. derive-authentication.py produced nothing for\n  this repo because there is no openapi/ directory.\napis:\n  - api: Parallax Evaluation API\n    schemes: []\n    model: none\n    transport_security: none-by-default\n    detail: >-\n      The Parallax server ships with NO authentication on either endpoint. The\n      axum router in src/server/api.rs registers POST /evaluate and GET /health\n      with no auth extractor or middleware,\
  \ and the shipped parallax.yaml binds\n      the listener to host 127.0.0.1 port 9920. Security is positional: the\n      server is expected to be reachable only from the agent process on the same\n      host (or inside the same pod/network namespace). There is no API key, no\n      bearer token, no mTLS option and no config key for one. Anyone who can\n      reach the port can submit evaluation events and read /health, which\n      discloses the running version and evaluator count.\n    recommendations:\n      - Do not bind Parallax to 0.0.0.0 without a fronting proxy that authenticates callers.\n      - Treat the absence of an auth option as a deployment constraint, not a defaults question.\n  - api: AI EdgeLabs Portal API\n    schemes:\n      - type: http\n        scheme: bearer\n        confirmed: false\n        note: >-\n          The API rejects anonymous requests, but the challenge is a JSON body,\n          not a WWW-Authenticate header, so the token type cannot be confirmed\n\
  \          without credentials.\n    model: session-or-token\n    federated_login:\n      - provider: Google\n        evidence: >-\n          The portal bundle requests the OAuth scopes\n          https://www.googleapis.com/auth/userinfo.email and\n          https://www.googleapis.com/auth/userinfo.profile.\n      - provider: GitHub\n        evidence: >-\n          The portal bundle constructs a https://github.com/login/oauth/authorize\n          request.\n    detail: >-\n      https://portal.edgelabs.ai/api/ and every path beneath it answered HTTP 401\n      with {\"message\":\"Unauthorized\",\"status\":401,\"errorCode\":101,\n      \"title\":\"Unauthorized\"} on 2026-08-13. No WWW-Authenticate header was\n      returned, no /.well-known/oauth-authorization-server or\n      /.well-known/openid-configuration document is served (both paths return the\n      SPA HTML shell, not a document), and no authentication documentation is\n      published. Sign-in to the console itself is federated\
  \ through Google and\n      GitHub OAuth; whether the same tokens authorize the API, or a separate key\n      is issued in-app, cannot be established without an account.\n    gated: true\noauth_scopes:\n  published: false\n  note: >-\n    No scope reference is published and no oauth2 flow is declared anywhere, so\n    no scopes/ artifact was written.\nsummary:\n  documented_auth_pages: 0\n  schemes_confirmed: 0\n  unauthenticated_surfaces: 1\n  gated_surfaces: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalarr/refs/heads/main/authentication/scalarr-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Cybersecurity
- Runtime Security
- AI Agent Security
- Container Security
- Kubernetes
- Edge Computing
- Vulnerability Management
- Compliance
- NIS2
- Machine Learning
- Artificial Intelligence
- Open Source
- Fraud Detection
- Mobile Ad Fraud
---
