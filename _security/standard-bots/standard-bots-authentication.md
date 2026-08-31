---
api_key_in: []
auth_types:
- http
description: Authentication profile for the RO1 Robotics REST API. The API runs on the robot control box and is authenticated with a Bearer token minted per robot from the Standard Bots app (Menu -> Settings -> Configure Developer API -> Enable Developer API). Every request also carries a robot-kind header selecting live vs simulated operation.
kind: authentication
layout: security
method: derived
name: Standard Bots Authentication
name_suffix: Authentication
oauth_flows: []
overview: Standard Bots secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Standard Bots
provider_slug: standard-bots
scheme_count: 1
schemes:
- description: 'Per-robot API token sent as `Authorization: Bearer <token>`. The token is generated in the Standard Bots app under Settings -> Configure Developer API, which also enables the Developer (Python/REST) API and optional ROS2 bridge on the control box. There is no OAuth authorization server and no scope surface; the token grants full Developer-API access to that robot.'
  name: bearerToken
  scheme: bearer
  sources:
  - packages/standard-bots-packages.yml
  type: http
slug: standard-bots-authentication
source_filename: standard-bots-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: >-\n  Derived from the official Standard Bots Python SDK (PyPI: standardbots 2.20260617.2,\n  standardbots.auto_generated.apis RequestManager.json_headers) and the\n  ros2-realtime-api README (developer API enablement). The RO1 docs REST-API site\n  is a single-page app with no downloadable OpenAPI, so the auth model is derived\n  from the first-party SDK rather than a spec.\ndescription: >-\n  Authentication profile for the RO1 Robotics REST API. The API runs on the robot\n  control box and is authenticated with a Bearer token minted per robot from the\n  Standard Bots app (Menu -> Settings -> Configure Developer API -> Enable Developer\n  API). Every request also carries a robot-kind header selecting live vs simulated\n  operation.\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    description: >-\n \
  \     Per-robot API token sent as `Authorization: Bearer <token>`. The token is\n      generated in the Standard Bots app under Settings -> Configure Developer API,\n      which also enables the Developer (Python/REST) API and optional ROS2 bridge\n      on the control box. There is no OAuth authorization server and no scope\n      surface; the token grants full Developer-API access to that robot.\n    sources:\n      - packages/standard-bots-packages.yml\nrequired_headers:\n  - name: Authorization\n    value: 'Bearer <token>'\n    required: true\n  - name: robot-kind\n    value: 'live | simulated'\n    required: true\n    description: >-\n      Selects the target robot context. `live` drives the physical RO1; `simulated`\n      targets a simulated robot (the SDK also accepts the legacy `robot_kind` header\n      for backwards compatibility).\n  - name: Content-Type\n    value: application/json\n    required: true\n    applies_to: request bodies\nenablement:\n  docs: https://standardbots.com/developers\n\
  \  steps:\n    - Open the Standard Bots app on the robot.\n    - Menu -> Settings -> Configure Developer API.\n    - Turn on \"Enable Developer API\" (enables the Python/REST API).\n    - Optionally turn on \"Enable ROS2 bridge\" for the realtime ROS2 topics.\n    - If \"Configure Developer API\" is missing, contact Standard Bots to enable it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-bots/refs/heads/main/authentication/standard-bots-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Robotics
- Industrial Automation
- Robotic Arm
- Manufacturing
- Artificial Intelligence
- Machine Tending
- Developer API
- ROS2
- Physical AI
---
