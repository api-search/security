---
api_key_in: []
api_specs:
- filename: bear-robotics-carti-api-openapi.yml
  format: yaml
  label: Bear Robotics Carti API
  slug: bear-robotics-carti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-carti-api-openapi.yml
- filename: bear-robotics-fleet-management-api-openapi.yml
  format: yaml
  label: Bear Robotics Fleet Management API
  slug: bear-robotics-fleet-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-fleet-management-api-openapi.yml
- filename: bear-robotics-localization-navigation-api-openapi.yml
  format: yaml
  label: Bear Robotics Localization & Navigation API
  slug: bear-robotics-localization-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-localization-navigation-api-openapi.yml
- filename: bear-robotics-locations-maps-api-openapi.yml
  format: yaml
  label: Bear Robotics Locations & Maps API
  slug: bear-robotics-locations-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-locations-maps-api-openapi.yml
- filename: bear-robotics-mission-api-openapi.yml
  format: yaml
  label: Bear Robotics Mission API
  slug: bear-robotics-mission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-mission-api-openapi.yml
- filename: bear-robotics-robot-status-api-openapi.yml
  format: yaml
  label: Bear Robotics Robot Status API
  slug: bear-robotics-robot-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-robot-status-api-openapi.yml
- filename: bear-robotics-robot-system-api-openapi.yml
  format: yaml
  label: Bear Robotics Robot System API
  slug: bear-robotics-robot-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-robot-system-api-openapi.yml
- filename: bear-robotics-servi-api-openapi.yml
  format: yaml
  label: Bear Robotics Servi API
  slug: bear-robotics-servi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-servi-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bear Robotics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bear Robotics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bear Robotics
provider_slug: bear-robotics
scheme_count: 1
schemes:
- applied: 'globally, via a root-level `security: [{BearerAuth: []}]` on all 23 operations'
  bearerFormat: JWT
  description: JWT token obtained from the /authorizeApiAccess endpoint
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/bear-robotics-cloud-openapi-original.yml
  type: http
slug: bear-robotics-authentication
source_filename: bear-robotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://cloud.api.bearrobotics.ai/guides/authentication/\ndocs: https://cloud.api.bearrobotics.ai/guides/authentication/\nderived_from: openapi/bear-robotics-cloud-openapi-original.yml\nsummary:\n  types:\n  - http\n  oauth2_flows: []\n  api_key_in: []\n  note: >-\n    A two-stage model that the OpenAPI securityScheme alone does not describe. The spec declares\n    only the second stage (an HTTP bearer JWT). The first stage — exchanging a long-lived API key\n    for that JWT at a separate host — is documented in prose and is not in any machine-readable\n    contract.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the /authorizeApiAccess endpoint\n  sources:\n  - openapi/bear-robotics-cloud-openapi-original.yml\n  applied: 'globally, via a root-level `security: [{BearerAuth: []}]` on all 23 operations'\ntoken_exchange:\n  endpoint: https://api-auth.bearrobotics.ai/authorizeApiAccess\n\
  \  method: POST\n  content_type: application/json\n  host_note: The auth host is separate from the API host (api.bearrobotics.ai).\n  credential_document:\n    fields:\n    - name: api_key\n      description: A unique identifier for the credentials within Bear's system.\n    - name: secret\n      description: A passcode associated with the API key; must be stored securely.\n    - name: scope\n      description: >-\n        Fixed at the time the API key is issued. Represents the distributor the API key is\n        authorized for. This is a tenancy identifier, NOT an OAuth scope — there is no scope\n        selection, no consent step and no per-permission granularity, so no scopes/ artifact is\n        emitted for this provider.\n    note: All three fields must match for the credentials to be authorized.\n  example_curl: |\n    curl -X POST https://api-auth.bearrobotics.ai/authorizeApiAccess \\\n        -H \"Content-Type: application/json\" \\\n        -d $(cat /path/to/credentials.json)\n\
  token_usage:\n  header: 'Authorization: Bearer <JWT>'\n  grpc: sent as gRPC call metadata on every outgoing request\n  rest: sent as a standard HTTP Authorization header\n  swagger_ui: the docs' Swagger UI accepts the JWT via its Authorize button\nexpiry:\n  claim: exp\n  guidance: refresh periodically, ideally every 30 minutes\n  refresh_mechanism: re-POST the credentials document; there is no refresh token\nauthorization_model:\n  boundary: distributor\n  granularity: all-or-nothing per distributor\n  note: >-\n    There are no scopes, roles or per-operation permissions. A credential either can act on a\n    robot or location or it cannot; calls referencing resources outside the distributor return\n    PERMISSION_DENIED. A key that can read robot status can also create missions and run system\n    commands — there is no read-only credential.\nprovisioning:\n  self_serve: false\n  process: API keys are issued by a Bear Robotics account manager\n  evidence: 'v1.3 changelog, New API Customers:\
  \ \"Please contact your Account Manager to discuss API use cases and request API keys.\"'\n  contact: https://www.bearrobotics.ai/contact-sales\ntransport:\n  tls: true\n  note: >-\n    All connections to the Bear Cloud API server are secured via TLS; server certificates are\n    signed by Google Trust Services. Probed 2026-08-06: api.bearrobotics.ai negotiates TLSv1.3.\n  exception: >-\n    The separate on-robot Bear Base API is documented with an insecure gRPC channel\n    (grpc.insecure_channel to 10.10.127.2:5123) over the robot's local ethernet link, and carries\n    no authentication of its own. Physical/network access to that link is the only control.\ndiscovery:\n  oidc: false\n  oauth_metadata: false\n  evidence: >-\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server return 404 on\n    www.bearrobotics.ai, api-auth.bearrobotics.ai and cloud.api.bearrobotics.ai, and 401 on\n    api.bearrobotics.ai (probed 2026-08-06). See well-known/bear-robotics-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/authentication/bear-robotics-authentication.yml
summary_line: http · 1 scheme
tags:
- Robotics
- Autonomous Mobile Robots
- Fleet Management
- Hospitality
- Food Service
- Logistics
- gRPC
- Protobuf
- Webhooks
- Internet of Things
- Company
---
