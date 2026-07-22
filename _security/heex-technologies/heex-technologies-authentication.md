---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Heex Technologies Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Heex Technologies secures its APIs with apiKey, oauth2, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Heex Technologies
provider_slug: heex-technologies
scheme_count: 4
schemes:
- description: USER_SECRET_KEY issued from the user's personal space on the Heex Cloud platform; required by the Heex CLI to operate the HeexSDK and interact with Heex Cloud.
  in: header
  name: UserSecretKey
  sources:
  - https://doc.heex.io/docs/command-line-interface/cli-overview
  type: apiKey
- description: API keys managed under Administration in the Heex web platform (interface-guide/administration/api-keys) for programmatic access.
  in: header
  name: PlatformAPIKeys
  sources:
  - https://doc.heex.io/docs/interface-guide/administration/api-keys
  type: apiKey
- description: OAuth 2.0 is used for platform logins (per the heex.io Security section).
  name: OAuth2
  scheme: authorizationCode
  sources:
  - https://www.heex.io/en-gb/security
  type: oauth2
- bearerFormat: JWT
  description: JWT bearer tokens are used for API authentication; agent-to-cloud communication is secured over HTTPS/TLS (per the heex.io Security section).
  name: BearerJWT
  scheme: bearer
  sources:
  - https://www.heex.io/en-gb/security
  type: http
slug: heex-technologies-authentication
source_filename: heex-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://doc.heex.io/docs/command-line-interface/cli-utilities/authentification\ndocs: https://doc.heex.io/docs/interface-guide/administration/api-keys\nnote: >-\n  No OpenAPI/Swagger is published by Heex, so this profile is captured from the\n  developer documentation (Docusaurus/Mintlify site at doc.heex.io) rather than\n  derived from a spec. The heex.io and doc.heex.io deployments were offline\n  (Vercel DEPLOYMENT_DISABLED / 404) at probe time; content verified via the\n  Internet Archive snapshots crawled through 2026-03.\nsummary:\n  types: [apiKey, oauth2, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: UserSecretKey\n    type: apiKey\n    in: header\n    description: >-\n      USER_SECRET_KEY issued from the user's personal space on the Heex Cloud\n      platform; required by the Heex CLI to operate the HeexSDK and interact with\n      Heex Cloud.\n    sources: [https://doc.heex.io/docs/command-line-interface/cli-overview]\n\
  \  - name: PlatformAPIKeys\n    type: apiKey\n    in: header\n    description: >-\n      API keys managed under Administration in the Heex web platform\n      (interface-guide/administration/api-keys) for programmatic access.\n    sources: [https://doc.heex.io/docs/interface-guide/administration/api-keys]\n  - name: OAuth2\n    type: oauth2\n    scheme: authorizationCode\n    description: >-\n      OAuth 2.0 is used for platform logins (per the heex.io Security section).\n    sources: [https://www.heex.io/en-gb/security]\n  - name: BearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      JWT bearer tokens are used for API authentication; agent-to-cloud\n      communication is secured over HTTPS/TLS (per the heex.io Security section).\n    sources: [https://www.heex.io/en-gb/security]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heex-technologies/refs/heads/main/authentication/heex-technologies-authentication.yml
summary_line: apiKey/oauth2/http · 4 schemes
tags:
- Company
- Autonomous Systems
- Robotics
- Autonomous Vehicles
- ADAS
- Data Management
- Edge Computing
- Fleet Monitoring
- Smart Data
- SDK
- CLI
---
