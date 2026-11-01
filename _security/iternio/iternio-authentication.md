---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Iternio Authentication
name_suffix: Authentication
oauth_flows: []
overview: A Better Route Planner (Iternio) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: A Better Route Planner (Iternio)
provider_slug: iternio
scheme_count: 1
schemes:
- authorizationUrl: https://abetterrouteplanner.com/oauth/auth?client_id=<your_client_id>&scope=<requested_scope>&response_type=code&redirect_uri=<your_redirect_uri>
  description: OAuth2 authentication for Iternio API
  scopes:
  - get_telemetry
  - set_telemetry
  - get_plan
  - vehicle_history
  tokenUrl: https://api.iternio.com/1/oauth/token?client_id=<your_client_id>&client_secret=<your_api_key>&code=<auth_code>
  type: oauth2
slug: iternio-authentication
source_filename: iternio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://abetterrouteplanner.com/resources/api\nschemes:\n  - type: oauth2\n    description: OAuth2 authentication for Iternio API\n    authorizationUrl: https://abetterrouteplanner.com/oauth/auth?client_id=<your_client_id>&scope=<requested_scope>&response_type=code&redirect_uri=<your_redirect_uri>\n    tokenUrl: https://api.iternio.com/1/oauth/token?client_id=<your_client_id>&client_secret=<your_api_key>&code=<auth_code>\n    scopes:\n      - get_telemetry\n      - set_telemetry\n      - get_plan\n      - vehicle_history"
source_yaml_url: https://artifacts.apis.io/iternio/authentication/iternio-authentication.yml
summary_line: 1 scheme
tags:
- Company
- EV
- Routing
- API
- Transportation
---
