---
api_key_in: []
api_specs:
- filename: tps-engage-play-api-openapi.yml
  format: yaml
  label: TPS Engage Play API
  slug: tps-engage-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/openapi/tps-engage-play-api-openapi.yml
- filename: tps-engage-prefetch-api-openapi.yml
  format: yaml
  label: TPS Engage Prefetch API
  slug: tps-engage-prefetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/openapi/tps-engage-prefetch-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Tps Engage Authentication
name_suffix: Authentication
oauth_flows: []
overview: TPS Engage declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: TPS Engage
provider_slug: tps-engage
scheme_count: 0
schemes: []
slug: tps-engage-authentication
source_filename: tps-engage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/tps-engage-blindspot-pull-api-openapi.yaml\ndocs: https://tpsengage.github.io/BlindspotPullApi/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  model: anonymous\n  statement: >-\n    The Blindspot Pull API — the only API TPS Engage publishes publicly — carries no\n    credential of any kind. The published OpenAPI 3.0.0 declares no\n    `components.securitySchemes` and no `security` requirement on either operation,\n    and no authentication is described anywhere in the hosted Swagger UI at\n    https://tpsengage.github.io/BlindspotPullApi/. Both operations were called\n    anonymously on 2026-08-13 against the production host and were served without a\n    401 or 403 (they returned 500 for the deviceId published in the spec's own\n    example). Authorization is therefore positional: the caller must possess a\n    registered `deviceId` UUID, which functions as an unguessable capability in the\n\
  \    URL path. That is a bearer-in-URL model with the usual consequences — the\n    identifier leaks into proxy logs, browser history and Referer headers, cannot be\n    scoped, and cannot be rotated without re-provisioning the player device.\n    The commercial platform behind the API (portal.seeblindspot.com) does have real\n    authentication — account sign-in at /auth/login, and the Trust & Security page\n    states \"Access control on a least-privilege basis, with multi-factor\n    authentication for administrative and remote access\" — but that is the buyer-side\n    web application, not an API credential, and no developer key issuance, OAuth\n    client registration or token endpoint is published.\nschemes: []\nobserved:\n- host: rtb.network.tpsengage.com\n  checked: '2026-08-13'\n  note: >-\n    GET /api/sv/play/{deviceId} and GET /api/sv/prefetch/{deviceId} called with no\n    Authorization header, no API key header and no cookie. Neither returned 401/403;\n    both returned 500.\
  \ No WWW-Authenticate header on any response.\n- host: rtb.network.tpsengage.com\n  checked: '2026-08-13'\n  note: >-\n    Response headers show a Helmet-style hardening baseline\n    (Strict-Transport-Security: max-age=31536000; includeSubDomains,\n    X-Content-Type-Options: nosniff, Referrer-Policy: no-referrer,\n    Content-Security-Policy, X-Frame-Options: SAMEORIGIN) with\n    access-control-allow-origin: * — an intentionally public, browser-callable\n    surface.\nidentifiers:\n- name: deviceId\n  in: path\n  format: uuid\n  required: true\n  role: capability\n  description: >-\n    Unique identifier of a registered player device on the Blindspot DOOH network.\n    Sole basis on which the API decides what to return. Provisioned to the screen\n    owner out of band during CMS integration; no self-service issuance is published.\n- name: apiPublisher\n  in: path\n  format: string\n  required: true\n  default: sv\n  role: routing\n  description: >-\n    Server variable in the base URL\
  \ (https://rtb.network.tpsengage.com/api/{apiPublisher}).\n    Names the publisher/CMS integration, not the caller; it is a routing segment, not\n    a credential.\ngaps:\n- No securitySchemes in the published OpenAPI.\n- No API key, OAuth 2.0, OIDC or mTLS surface published for the Pull API.\n- No token rotation, expiry or revocation story for a compromised deviceId.\n- >-\n  No scope model — a deviceId grants exactly the playback slice for that one screen,\n  which is a small blast radius, but there is nothing to scope down further and\n  nothing to scope up for a multi-screen operator.\n- >-\n  Portal (buyer-side) API access is not documented at all; the full API is described\n  in Blindspot's own marketing as available \"reach out to set up a demo\", so any\n  campaign/booking API sits behind a sales gate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/authentication/tps-engage-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- DOOH
- Digital Billboards
- Programmatic Advertising
- Media Buying
- Out-of-Home
---
