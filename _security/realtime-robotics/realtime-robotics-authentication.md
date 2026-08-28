---
api_key_in: []
auth_types: []
description: 'Realtime Robotics publishes no OpenAPI, so this profile is assembled from the documentation for each of its three surfaces plus a live probe of the identity service and the application API gateway. The picture is sharply split: the cloud application is behind a real OpenID Connect provider, while the two on-premise controller APIs document no authentication at all and rely on plant-network isolation.'
kind: authentication
layout: security
method: searched
name: Realtime Robotics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Realtime Robotics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Realtime Robotics
provider_slug: realtime-robotics
scheme_count: 0
schemes: []
slug: realtime-robotics-authentication
source_filename: realtime-robotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://resolver.rtr.ai/docs/user_guide/resolver/request_account/\ndocs: https://resolver.rtr.ai/docs/user_guide/resolver/log_in/\nname: Realtime Robotics authentication profile\ndescription: >-\n  Realtime Robotics publishes no OpenAPI, so this profile is assembled from the\n  documentation for each of its three surfaces plus a live probe of the identity\n  service and the application API gateway. The picture is sharply split: the cloud\n  application is behind a real OpenID Connect provider, while the two on-premise\n  controller APIs document no authentication at all and rely on plant-network\n  isolation.\nsurfaces:\n- api: realtime-robotics:resolver-cloud\n  name: Resolver Cloud\n  scheme: openIdConnect\n  provider: Clerk, served on the company's own subdomain clerk.rtr.ai\n  openid_configuration: https://clerk.rtr.ai/.well-known/openid-configuration\n  issuer: https://clerk.rtr.ai\n  authorization_endpoint: https://clerk.rtr.ai/oauth/authorize\n\
  \  token_endpoint: https://clerk.rtr.ai/oauth/token\n  userinfo_endpoint: https://clerk.rtr.ai/oauth/userinfo\n  jwks_uri: https://clerk.rtr.ai/.well-known/jwks.json\n  revocation_endpoint: https://clerk.rtr.ai/oauth/token/revoke\n  introspection_endpoint: https://clerk.rtr.ai/oauth/token_info\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  pkce:\n    supported: true\n    methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  id_token_signing_alg:\n  - RS256\n  onboarding: >-\n    Accounts are not self-service. The documentation states an account must be\n    requested with a corporate email address, first name, last name and company;\n    Realtime Robotics then creates it and sends a temporary password from\n    no-reply@verificationemail.com which the user changes on first login.\n  api_gateway_probe:\n    url: https://app.resolver.rtr.ai/api/openapi.json\n    http_status: 403\n   \
  \ body: '{\"message\":\"Missing Authentication Token\"}'\n    reading: >-\n      The application's /api surface is an authenticated AWS API Gateway. Anonymous\n      callers are rejected; no public credential model for it is documented, which is\n      consistent with the docs saying the public REST API is not yet available.\n  method: probed\n- api: realtime-robotics:rapidplan-ascii-api\n  name: RapidPlan Realtime Controller ASCII API\n  scheme: none\n  evidence: >-\n    The 2.9 ASCII API reference documents the full request envelope\n    ({topic, type, id, data}) with no authentication, credential, token or key field,\n    and the first-party Python examples connect with PythonCommander(ip_addr, 9999)\n    over a raw TCP socket with no credential. GetRapidSenseStatus is documented as\n    callable \"as soon as the RTR controller accepts a socket\".\n  control: >-\n    Access control is network-level - the Realtime Controller is an on-premise\n    appliance on the cell network. Nothing\
  \ in the published documentation authenticates\n    or authorises an individual client.\n  method: searched\n  source: https://realtimerobotics.atlassian.net/wiki/spaces/rapidplandocs/pages/3467120890/2.9+Realtime+Robotics+RapidPlan+ASCII+API\n- api: realtime-robotics:rapidsense-api\n  name: RapidSense API\n  scheme: none\n  evidence: >-\n    The 2.9 RapidSense API reference documents the REST interface on port 11235 with\n    request/response bodies and HTTP status codes but no Authorization header, API key,\n    or auth scheme on any endpoint.\n  control: network-level only, same on-premise posture as the ASCII API\n  method: searched\n  source: https://realtimerobotics.atlassian.net/wiki/spaces/rapidplandocs/pages/3467120157/2.9+RapidSense+API\ngaps:\n- No API keys, personal access tokens or machine credentials are documented for any\n  surface.\n- No mutual TLS, signed-request or fieldbus authentication is documented for the\n  PROFINET or CC-Link IE Field Basic interfaces.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtime-robotics/refs/heads/main/authentication/realtime-robotics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Robotics
- Motion Planning
- Industrial Automation
- Manufacturing
- Simulation
- Collision Avoidance
- Robot Programming
- Machine Vision
- Digital Twin
---
