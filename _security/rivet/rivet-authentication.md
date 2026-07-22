---
api_key_in: []
api_specs:
- filename: rivet-rivetkit-openapi.json
  format: json
  label: RivetKit API
  slug: rivetkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivet/refs/heads/main/openapi/rivet-rivetkit-openapi.json
auth_types:
- bearer
- custom-token
description: ''
kind: authentication
layout: security
method: searched
name: Rivet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rivet secures its APIs with bearer and custom-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rivet
provider_slug: rivet
scheme_count: 2
schemes:
- description: Rivet Cloud API token (prefix cloud_api_) used by the CLI and management API to deploy and manage projects.
  name: CloudApiToken
  plane: cloud-management
  scheme: bearer
  source: https://www.rivet.dev/docs/cli
  type: http
- description: Application-defined token validated in the actor onBeforeConnect / createConnState hooks; authorization enforced by access-control hooks.
  in: connection-params
  name: authToken
  plane: actor-gateway
  source: https://www.rivet.dev/docs/actors/access-control
  type: apiKey
slug: rivet-authentication
source_filename: rivet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.rivet.dev/docs/actors/access-control\ndocs: https://www.rivet.dev/docs/actors/access-control\nsummary:\n  types: [bearer, custom-token]\n  notes: >-\n    Rivet uses two distinct planes. (1) The Rivet Cloud management/deploy plane\n    authenticates with a Cloud API token (prefix `cloud_api_`), passed to the\n    CLI via `rivet deploy --token cloud_api_xxxxx` and stored locally for\n    subsequent deploys — a bearer-style secret. (2) The RivetKit actor gateway\n    is application-authenticated: clients pass an `authToken` (or arbitrary\n    params) through connection parameters that your actor validates in the\n    `onBeforeConnect` / `createConnState` hooks, and enforces per-action,\n    per-queue (`canPublish`) and per-event (`canSubscribe`) with a deny-by-default\n    access-control model. The published OpenAPI declares no `securitySchemes`\n    (gateway auth is defined by the developer's own hooks), but gateway\n\
  \    operations return 401 Unauthorized when a request is not authorized.\nschemes:\n  - name: CloudApiToken\n    type: http\n    scheme: bearer\n    description: >-\n      Rivet Cloud API token (prefix cloud_api_) used by the CLI and management\n      API to deploy and manage projects.\n    plane: cloud-management\n    source: https://www.rivet.dev/docs/cli\n  - name: ActorConnectionAuth\n    type: apiKey\n    in: connection-params\n    name: authToken\n    description: >-\n      Application-defined token validated in the actor onBeforeConnect /\n      createConnState hooks; authorization enforced by access-control hooks.\n    plane: actor-gateway\n    source: https://www.rivet.dev/docs/actors/access-control\nobserved_status_codes:\n  - {code: 401, meaning: Unauthorized, operations: 10}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rivet/refs/heads/main/authentication/rivet-authentication.yml
summary_line: bearer/custom-token · 2 schemes
tags:
- Company
- Infrastructure
- Actors
- Stateful Compute
- AI Agents
- Realtime
- Serverless
- Edge
- WebSockets
- Durable Execution
- Developer Tools
---
