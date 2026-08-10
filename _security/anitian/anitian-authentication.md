---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Anitian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anitian declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Anitian
provider_slug: anitian
scheme_count: 0
schemes: []
slug: anitian-authentication
source_filename: anitian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://securecloud.anitian.com/api/auth/providers\nname: Anitian authentication profile\nsummary: >-\n  Anitian publishes no developer authentication documentation, no API key model, and\n  no OAuth scope reference. Everything below was observed by probing the live hosts\n  anonymously. The SecureCloud / FedFlex console is a Next.js application using\n  NextAuth with two federated OAuth/OIDC identity providers; every application and\n  API path behind it redirects unauthenticated callers to the sign-in page. The\n  FedFlex copilot WebSocket API is fronted by an AWS API Gateway custom authorizer.\n\nhosts:\n\n  - host: securecloud.anitian.com\n    surface: Anitian SecureCloud / FedFlex console + platform API\n    model: federated-oauth-session\n    session:\n      framework: NextAuth.js\n      cookies:\n        - name: __Host-next-auth.csrf-token\n          attributes: [Path=/, HttpOnly, Secure, 'SameSite=Lax']\n        - name:\
  \ __Secure-next-auth.callback-url\n          attributes: [Path=/, HttpOnly, Secure, 'SameSite=Lax']\n      csrf_endpoint: https://securecloud.anitian.com/api/auth/csrf\n      session_endpoint: https://securecloud.anitian.com/api/auth/session\n    identity_providers:\n      - id: okta\n        name: Okta\n        type: oauth\n        signin_url: https://securecloud.anitian.com/api/auth/signin/okta\n        callback_url: https://securecloud.anitian.com/api/auth/callback/okta\n      - id: cognito\n        name: Amazon Cognito\n        type: oauth\n        signin_url: https://securecloud.anitian.com/api/auth/signin/cognito\n        callback_url: https://securecloud.anitian.com/api/auth/callback/cognito\n    anonymous_endpoints:\n      - path: /api/health\n        status: 200\n        body: '{\"status\":\"ok\",\"version\":\"\"}'\n      - path: /api/auth/providers\n        status: 200\n        note: enumerates the two OAuth providers\n      - path: /api/auth/csrf\n        status: 200\n     \
  \ - path: /api/auth/session\n        status: 200\n        body: '{}'\n    gated_behaviour:\n      redirect: 307 -> /auth/signin?callbackUrl=<original path>\n      note: >-\n        Applies to every other path probed, including /api, /openapi.json,\n        /swagger.json, /api-docs, /docs, /redoc, /graphql, /mcp, /llms.txt and\n        every /.well-known/* path. The console answers 307 rather than 401/403,\n        so no WWW-Authenticate challenge and no OAuth metadata is exposed.\n\n  - host: copilot.anitian.com\n    surface: Anitian FedFlex Copilot WebSocket API\n    model: apigateway-custom-authorizer\n    infrastructure: AWS API Gateway (WebSocket), us-west-2\n    observed:\n      - probe: plain HTTPS GET on any path\n        status: 426\n        headers: 'sec-websocket-version: 13'\n      - probe: WebSocket upgrade handshake (Connection/Upgrade/Sec-WebSocket-Key)\n        status: 401\n        body: '{\"message\": \"Unauthorized\", \"connectionId\": \"...\", \"requestId\": \"...\"}'\n\
  \        note: >-\n          $connect route rejected. Credential form (query-string token, header,\n          or IAM SigV4) is not documented anywhere public.\n\nnot_found:\n  - what: OpenID Connect discovery\n    probed:\n      - url: https://www.anitian.com/.well-known/openid-configuration\n        status: 404\n      - url: https://securecloud.anitian.com/.well-known/openid-configuration\n        status: 307\n  - what: OAuth authorization-server metadata (RFC 8414)\n    probed:\n      - url: https://www.anitian.com/.well-known/oauth-authorization-server\n        status: 404\n      - url: https://securecloud.anitian.com/.well-known/oauth-authorization-server\n        status: 307\n  - what: OAuth protected-resource metadata (RFC 9728)\n    probed:\n      - url: https://securecloud.anitian.com/.well-known/oauth-protected-resource\n        status: 307\n  - what: API keys, personal access tokens, or a documented machine-to-machine flow\n    note: >-\n      None documented. Anitian's own FedRAMP\
  \ 20x README states \"an API is available\n      for auditors to download evidence and integrate it into their own systems\",\n      but neither the endpoint nor its credential model is published.\n\nx-evidence:\n  fetched: '2026-08-06'\n  method: anonymous HTTP probes, no credentials used\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anitian/refs/heads/main/authentication/anitian-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Security
- Compliance
- Cloud
- Governance
- FedRAMP
- Government
- Risk
- Audit
- Automation
---
