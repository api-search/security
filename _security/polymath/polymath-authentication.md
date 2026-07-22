---
api_key_in: []
api_specs:
- filename: polymath-synapse-v2-openapi-original.json
  format: json
  label: Polymath Synapse API
  slug: polymath-synapse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-synapse-v2-openapi-original.json
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
