---
api_key_in: []
api_specs:
- filename: polymath-canbus-api-openapi.yml
  format: yaml
  label: Polymath Robotics CANBus API
  slug: polymath-canbus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-canbus-api-openapi.yml
- filename: polymath-filesystem-api-openapi.yml
  format: yaml
  label: Polymath Robotics filesystem API
  slug: polymath-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-filesystem-api-openapi.yml
- filename: polymath-health-check-api-openapi.yml
  format: yaml
  label: Polymath Robotics Health Check API
  slug: polymath-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-health-check-api-openapi.yml
- filename: polymath-livekit-api-openapi.yml
  format: yaml
  label: Polymath Robotics Livekit API
  slug: polymath-livekit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-livekit-api-openapi.yml
- filename: polymath-media-api-openapi.yml
  format: yaml
  label: Polymath Robotics Media API
  slug: polymath-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-media-api-openapi.yml
- filename: polymath-ros-api-openapi.yml
  format: yaml
  label: Polymath Robotics ros API
  slug: polymath-ros-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-ros-api-openapi.yml
- filename: polymath-systemd-api-openapi.yml
  format: yaml
  label: Polymath Robotics systemd API
  slug: polymath-systemd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-systemd-api-openapi.yml
- filename: polymath-teleop-control-api-openapi.yml
  format: yaml
  label: Polymath Robotics Teleop Control API
  slug: polymath-teleop-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-teleop-control-api-openapi.yml
- filename: polymath-vehicle-autonomy-api-openapi.yml
  format: yaml
  label: Polymath Robotics Vehicle Autonomy API
  slug: polymath-vehicle-autonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-vehicle-autonomy-api-openapi.yml
- filename: polymath-vehicle-operations-api-openapi.yml
  format: yaml
  label: Polymath Robotics Vehicle Operations API
  slug: polymath-vehicle-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-vehicle-operations-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Polymath Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Polymath Robotics secures its APIs with oauth2 and http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Polymath Robotics
provider_slug: polymath
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/polymath-synapse-v2-openapi-original.json
  type: http
slug: polymath-authentication
source_filename: polymath-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/polymath-synapse-v2-openapi-original.json\ndocs: https://synapse.docs.polymathrobotics.dev/docs/guides/authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    The Synapse OpenAPI declares an HTTP Bearer security scheme (HTTPBearer).\n    The authentication guide documents that the bearer token is obtained via an\n    OAuth 2.0 client-credentials flow against the Polymath identity host, then\n    presented as `Authorization: Bearer <access_token>` on every Synapse call.\noauth2:\n  grant_type: client_credentials\n  token_url: https://polyglot.polymathrobotics.dev/oauth/token\n  audience: https://api.polymathrobotics.dev/\n  request_fields:\n  - client_id\n  - client_secret\n  - audience\n  - grant_type\n  response_token_field: access_token\n  credentials_required:\n  - client_id\n  - client_secret\n  - device_id\n  gateway: https://polyglot.polymathrobotics.dev/api/synapse/{DEVICE_ID}/v2\n\
  \  scopes: none documented\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/polymath-synapse-v2-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/authentication/polymath-authentication.yml
summary_line: oauth2/http · 1 scheme
tags:
- Robotics
- Autonomy
- Industrial Vehicles
- Off-Highway
- Machine Learning
- Simulation
- Teleoperation
- Automation
- Artificial Intelligence
- Unmanned Vehicles
---
