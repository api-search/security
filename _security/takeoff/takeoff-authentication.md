---
api_key_in: []
auth_types: []
description: Takeoff Technologies publishes no developer portal, no API reference and no machine-readable contract anywhere on the public web, but api.takeoff.com is a live, actively-maintained API gateway. This profile is what could be established about its authentication model from OUTSIDE the wall, by unauthenticated probing only. It is NOT derived from a provider-published specification, and nothing here should be read as documentation Takeoff publishes — no `Authentication` pointer is wired into apis.yml for exactly that reason.
kind: authentication
layout: security
method: probed
name: Takeoff Authentication
name_suffix: Authentication
oauth_flows: []
overview: TakeOff declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: TakeOff
provider_slug: takeoff
scheme_count: 0
schemes: []
slug: takeoff-authentication
source_filename: takeoff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://api.takeoff.com/ — unauthenticated HTTP probes, 2026-08-29\ndescription: >-\n  Takeoff Technologies publishes no developer portal, no API reference and no\n  machine-readable contract anywhere on the public web, but api.takeoff.com is a\n  live, actively-maintained API gateway. This profile is what could be\n  established about its authentication model from OUTSIDE the wall, by\n  unauthenticated probing only. It is NOT derived from a provider-published\n  specification, and nothing here should be read as documentation Takeoff\n  publishes — no `Authentication` pointer is wired into apis.yml for exactly\n  that reason.\nhost: https://api.takeoff.com\ngateway:\n  platform: Google Cloud (via 1.1 google, HTTP/2, alt-svc h3)\n  certificate_issuer: Google Trust Services WR3\n  certificate_reissued: '2026-07-16'\n  default_response: HTTP 404 with a zero-length body for any unrouted path\n  request_correlation: >-\n    Every\
  \ routed response carries an `x-request-id` header holding a UUIDv4 —\n    a real request-tracing convention, observable without credentials.\nobserved_schemes:\n  - scheme: unknown-header\n    evidence: >-\n      HTTP 401 application/json {\"code\":\"401\", \"message\":\"Missing authentication\n      header.\"} on every path under /auth/ and /sites/. The gateway names the\n      requirement (\"authentication header\") but does not name the header, the\n      scheme, or a token endpoint, and returns no WWW-Authenticate header.\n    www_authenticate: null\n    note: >-\n      No OAuth metadata is served: /.well-known/oauth-authorization-server,\n      /.well-known/oauth-protected-resource and /.well-known/openid-configuration\n      all 404 on this host, and /oauth, /oauth2, /token and /sso are unrouted.\n      Whether the scheme is bearer, an API key header, or mTLS cannot be\n      determined from outside.\nroutes_observed:\n  - path: /auth\n    status: 401\n    body: '{\"code\":\"401\"\
  , \"message\":\"Missing authentication header.\"}'\n    note: >-\n      Prefix routes — every child path probed (/auth/, /auth/login, /auth/v1,\n      /auth/health, /auth/openapi.json, /auth/api-docs, /auth/v3/api-docs,\n      /auth/swagger-ui.html, /auth/actuator/health) returns the same 401, so no\n      spec or health endpoint is reachable unauthenticated.\n  - path: /auth/token\n    status: 404\n    body: '{\"code\":\"404\", \"message\":\"Path not found : /auth/token\"}'\n    note: >-\n      A DIFFERENT 404 shape from the gateway default — a JSON body naming the\n      path. This proves routing exists inside /auth and that the 404 is issued\n      by the service, not by the load balancer.\n  - path: /sites\n    status: 401\n    body: '{\"code\":\"401\", \"message\":\"Missing authentication header.\"}'\n  - path: /webhooks\n    status: 403\n    body: '{\"message\":\"Forbidden\", \"path\": \"\"}'\n    note: >-\n      A webhook surface exists behind the gateway. It is NOT publicly\n \
  \     documented, so no `Webhooks` pointer is wired.\n  - path: /identity\n    status: 403\n    body: '{\"message\":\"Forbidden\", \"path\": \"\"}'\nunrouted_probed:\n  note: >-\n    All of these returned the gateway default (404, zero-length body), i.e. no\n    such route is published at the edge.\n  paths:\n    - /\n    - /v1\n    - /v2\n    - /v3\n    - /api\n    - /api/v1\n    - /docs\n    - /developer\n    - /graphql\n    - /mcp\n    - /openapi.json\n    - /openapi.yaml\n    - /swagger.json\n    - /api-docs\n    - /swagger-ui\n    - /health\n    - /healthz\n    - /status\n    - /ping\n    - /version\n    - /metrics\n    - /login\n    - /oauth\n    - /oauth2\n    - /token\n    - /sso\n    - /orders\n    - /inventory\n    - /catalog\n    - /users\n    - /products\n    - /items\n    - /picking\n    - /fulfillment\n    - /stores\n    - /wms\n    - /oms\n    - /events\n    - /admin\n    - /gateway\n    - /public\n    - /partner\n    - /integrations\n    - /reports\n    - /analytics\n \
  \   - /notifications\n    - /config\n    - /tenants\n    - /accounts\n    - /devices\n    - /telemetry\n    - /mfc\nlimits:\n  - No credentials were used and none were sought; nothing behind the wall was accessed.\n  - >-\n    The header name, token format, scope model, expiry and refresh behaviour are\n    all unknown and are deliberately left unrecorded rather than guessed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/takeoff/refs/heads/main/authentication/takeoff-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Grocery
- Retail
- eCommerce
- Fulfillment
- Micro-Fulfillment
- Warehouse Automation
- Robotics
- Supply Chain
- Logistics
---
