---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Wandelbots Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wandelbots declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Wandelbots
provider_slug: wandelbots
scheme_count: 1
schemes:
- description: 'Per-instance access token issued in the Wandelbots NOVA Developer Portal.

    Passed as an Authorization: Bearer <token> header on NOVA API requests and via

    the NOVA_ACCESS_TOKEN environment variable when using the Python/TypeScript

    SDKs. Mandatory for the Wandelbots Cloud environment; local/on-prem instances

    may be reachable without a token depending on deployment.

    '
  env: NOVA_ACCESS_TOKEN
  format: Bearer <access token>
  header: Authorization
  id: nova_access_token
  in: header
  scheme: bearer
  type: http
slug: wandelbots-authentication
source_filename: wandelbots-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: |\n  Wandelbots NOVA API documentation (docs.wandelbots.io/*/nova-api) and the NOVA\n  SDK README (github.com/wandelbotsgmbh/wandelbots-nova). Documented auth: an\n  access token issued per-instance in the Developer Portal, supplied to the API /\n  SDK as a bearer token (env var NOVA_ACCESS_TOKEN, mandatory for the Wandelbots\n  Cloud environment).\ndocs: https://docs.wandelbots.io/25.9/nova-api\nprovider: Wandelbots\napi: Wandelbots NOVA API\nschemes:\n- id: nova_access_token\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer <access token>\n  env: NOVA_ACCESS_TOKEN\n  description: |\n    Per-instance access token issued in the Wandelbots NOVA Developer Portal.\n    Passed as an Authorization: Bearer <token> header on NOVA API requests and via\n    the NOVA_ACCESS_TOKEN environment variable when using the Python/TypeScript\n    SDKs. Mandatory for the Wandelbots Cloud environment; local/on-prem\
  \ instances\n    may be reachable without a token depending on deployment.\ndefault_scheme: nova_access_token\nnotes: |\n  The NOVA API is served from each NOVA instance (Cloud or on-prem appliance) at\n  <instance-host>/api/v2. There is no public multi-tenant OAuth2 authorization\n  server documented; authentication is a portal-issued bearer access token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wandelbots/refs/heads/main/authentication/wandelbots-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Software Automation
- Robotics
- Industrial Automation
- Robot Programming
- Motion Planning
- Physical AI
- SDK
---
