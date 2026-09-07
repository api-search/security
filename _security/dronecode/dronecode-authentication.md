---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Dronecode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dronecode Foundation declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Dronecode Foundation
provider_slug: dronecode
scheme_count: 0
schemes: []
slug: dronecode-authentication
source_filename: dronecode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  derive-authentication.py found nothing (there is no OpenAPI to read). Written instead from the 39\n  verbatim MAVSDK protobuf contracts under grpc/, from the MAVSDK/PX4 guides, and from a live\n  unauthenticated probe of https://dronecode.org/wp-json/ and its wp-abilities routes on 2026-09-06.\nprovider: Dronecode Foundation\nproviderId: dronecode\nsummary: >-\n  Two very different surfaces. The MAVSDK gRPC contract — the real API — declares NO authentication at\n  all, by design: the consumer runs the server themselves. The dronecode.org WordPress REST API, which\n  the Foundation's own /.well-known/api-catalog advertises, authenticates with WordPress Application\n  Passwords and refuses anonymous callers on everything but the discovery document.\nsurfaces:\n  - api: MAVSDK gRPC API\n    contract: grpc/_index.yml\n    schemes: []\n    scheme_count: 0\n    transport_security: none\n    detail: >-\n      No securityScheme\
  \ equivalent appears in any of the 39 protos. mavsdk_server accepts plaintext\n      gRPC on 0.0.0.0:50051 with no TLS, no token, no mTLS and no per-call credential, and the\n      contract defines no scopes. This is not an omission the provider could close in the contract:\n      the server is a binary the CONSUMER runs on their own machine or companion computer, so the\n      trust boundary is the network they place it on, not a credential the Foundation issues.\n    consequences:\n      - >-\n        Anything that can reach port 50051 can arm, take off, and terminate the aircraft. The\n        ActionService contract has Arm, ArmForce, Kill and Terminate and none of them are gated.\n      - >-\n        There is no delegated identity, no consent surface, and no way to distinguish one caller from\n        another — every request is anonymous and fully privileged.\n      - >-\n        Binding mavsdk_server to anything other than loopback, or to a network an untrusted party can\n       \
  \ reach, is an unauthenticated remote flight-control surface.\n    mitigation_documented: >-\n      The MAVSDK guide documents the --port/bind arguments and the usual deployment is loopback or a\n      dedicated companion-computer link, but no authentication guidance is published as part of the\n      contract.\n    docs: https://mavsdk.mavlink.io/main/en/\n  - api: dronecode.org WordPress REST API\n    contract: null\n    baseURL: https://dronecode.org/wp-json/\n    schemes:\n      - type: http\n        scheme: application-password\n        name: WordPress Application Passwords\n        location: Authorization header (HTTP Basic, user + application password)\n        authorization_endpoint: https://dronecode.org/wp-admin/authorize-application.php\n        source: >-\n          Read verbatim from the `authentication` block of the API's own discovery document at\n          https://dronecode.org/wp-json/ (HTTP 200, application/json, probed 2026-09-06).\n    scheme_count: 1\n    oauth2: false\n\
  \    openid_connect: false\n    detail: >-\n      The discovery root is anonymous and lists 74 routes across 7 namespaces. Everything behind it is\n      not. The wp/v2 content namespace is declared in `namespaces` but its routes are absent from the\n      route index and /wp-json/wp/v2/posts returns rest_no_route (404) — the content API has been\n      switched off rather than left open. /wp-json/wp-abilities/v1/abilities, the WordPress Abilities\n      API (an agent-callable tool surface, with a POST .../run endpoint), returns rest_forbidden 401\n      anonymously.\n    probes:\n      - url: https://dronecode.org/wp-json/\n        status: 200\n        note: 74 routes, namespaces yoast/v1, objectcache/v1, regenerate-thumbnails/v1, wp/v2, wp-site-health/v1, wp-block-editor/v1, wp-abilities/v1\n      - url: https://dronecode.org/wp-json/wp/v2/posts?per_page=1\n        status: 404\n        note: '{\"code\":\"rest_no_route\"} — the wp/v2 content routes are not registered'\n      - url: https://dronecode.org/wp-json/wp-abilities/v1/abilities\n\
  \        status: 401\n        note: '{\"code\":\"rest_forbidden\"} — the Abilities (agent tool) surface requires authentication'\n    docs: https://developer.wordpress.org/rest-api/\n    docs_note: >-\n      Third-party (WordPress core) documentation, not Dronecode's — but it is exactly what the\n      Foundation's own /.well-known/api-catalog names as this API's service-doc.\ngaps:\n  - No OAuth 2.0, OpenID Connect, or delegated-identity surface anywhere in the estate.\n  - No scopes, so scopes/ is genuinely N/A rather than missing.\n  - >-\n    No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource on any of the\n    eight hosts probed — all 404. See well-known/dronecode-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dronecode/refs/heads/main/authentication/dronecode-authentication.yml
summary_line: 0 schemes
tags:
- Drones
- UAV
- Robotics
- MAVLink
- PX4
- Autopilot
- Aerial Robotics
- gRPC
- Open Source
- Linux Foundation
---
