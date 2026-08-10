---
api_key_in:
- header
api_specs:
- filename: tapcart-development-api-block-templates-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Block Templates API
  slug: tapcart-development-api-block-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-block-templates-api-openapi.yml
- filename: tapcart-development-api-blocks-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Blocks API
  slug: tapcart-development-api-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-blocks-api-openapi.yml
- filename: tapcart-development-api-components-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Components API
  slug: tapcart-development-api-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-components-api-openapi.yml
- filename: tapcart-development-api-dependencies-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Dependencies API
  slug: tapcart-development-api-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-dependencies-api-openapi.yml
- filename: tapcart-development-api-layouts-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Layouts API
  slug: tapcart-development-api-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-layouts-api-openapi.yml
auth_types:
- http
- apiKey
description: 'Tapcart''s authentication surface is not uniform: the three public API surfaces each use a different credential. The Development API (App Studio) declares HTTP bearer with a JWT in its OpenAPI and applies it globally. The Insights Metrics API uses a static per-organization api-key header alongside an app-id header. The CLI and its bundled MCP server authenticate a human through an Auth0 browser login and cache the result in ~/.tapcart/auth.json. The published auth page documents the first two interchangeably ("Authorization: Bearer ${accessToken}" or "api-key"), without stating which surface takes which.'
kind: authentication
layout: security
method: searched
name: Tapcart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tapcart secures its APIs with http and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tapcart
provider_slug: tapcart
scheme_count: 5
schemes:
- applies_to: Tapcart App Studio Development API (https://api.tapcart.com)
  bearerFormat: JWT
  declared_globally: true
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tapcart-client-api-openapi-original.json
  type: http
- applies_to: Tapcart Insights Metrics API (https://api.tapcart.com/insights-pro/v2/metrics)
  description: '"A static key with authorized access for your organization." Merchants without access are told to contact Tapcart support — the key is not self-service issuable.'
  in: header
  name: api-key
  parameter_name: api-key
  sources:
  - https://dev.tapcart.com/reference/insights-api
  type: apiKey
- description: The organization's Tapcart app id. Documented as good practice on all requests; must match the appId in the request body when using session-based auth. Not a credential on its own.
  in: header
  name: app-id
  parameter_name: app-id
  role: tenant-selector
  sources:
  - https://dev.tapcart.com/reference/insights-api
  type: apiKey
- description: Declared as a reusable header parameter in components.parameters but not referenced by any published operation. Present in the spec, unused by the documented surface.
  in: header
  name: installation-id
  parameter_name: installation-id
  role: reusable-parameter
  sources:
  - openapi/tapcart-client-api-openapi-original.json
  type: apiKey
- description: Declared as a reusable header parameter in components.parameters but not referenced by any published operation. Implies a session-based auth mode alongside the bearer JWT.
  in: header
  name: session-token
  parameter_name: session-token
  role: reusable-parameter
  sources:
  - openapi/tapcart-client-api-openapi-original.json
  type: apiKey
slug: tapcart-authentication
source_filename: tapcart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/tapcart-client-api-openapi-original.json\ndocs: https://dev.tapcart.com/reference/api-setup-and-auth\ndescription: >-\n  Tapcart's authentication surface is not uniform: the three public API\n  surfaces each use a different credential. The Development API (App Studio)\n  declares HTTP bearer with a JWT in its OpenAPI and applies it globally. The\n  Insights Metrics API uses a static per-organization api-key header alongside\n  an app-id header. The CLI and its bundled MCP server authenticate a human\n  through an Auth0 browser login and cache the result in ~/.tapcart/auth.json.\n  The published auth page documents the first two interchangeably\n  (\"Authorization: Bearer ${accessToken}\" or \"api-key\"), without stating which\n  surface takes which.\nsummary:\n  types: [http, apiKey]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    No oauth2 or openIdConnect security scheme is declared\
  \ in any published\n    spec, and no scope or permission reference page exists — so no scopes/\n    artifact was written. The CLI's Auth0 login is a human interactive flow,\n    not a documented machine OAuth grant; no\n    /.well-known/oauth-authorization-server or\n    /.well-known/oauth-protected-resource is served on any Tapcart host (all\n    404, see well-known/tapcart-well-known.yml).\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to: Tapcart App Studio Development API (https://api.tapcart.com)\n    declared_globally: true\n    sources:\n      - openapi/tapcart-client-api-openapi-original.json\n  - name: api-key\n    type: apiKey\n    in: header\n    parameter_name: api-key\n    applies_to: Tapcart Insights Metrics API (https://api.tapcart.com/insights-pro/v2/metrics)\n    description: >-\n      \"A static key with authorized access for your organization.\" Merchants\n      without access are told to contact Tapcart support\
  \ — the key is not\n      self-service issuable.\n    sources:\n      - https://dev.tapcart.com/reference/insights-api\n  - name: app-id\n    type: apiKey\n    in: header\n    parameter_name: app-id\n    role: tenant-selector\n    description: >-\n      The organization's Tapcart app id. Documented as good practice on all\n      requests; must match the appId in the request body when using\n      session-based auth. Not a credential on its own.\n    sources:\n      - https://dev.tapcart.com/reference/insights-api\n  - name: installation-id\n    type: apiKey\n    in: header\n    parameter_name: installation-id\n    role: reusable-parameter\n    description: >-\n      Declared as a reusable header parameter in components.parameters but not\n      referenced by any published operation. Present in the spec, unused by the\n      documented surface.\n    sources:\n      - openapi/tapcart-client-api-openapi-original.json\n  - name: session-token\n    type: apiKey\n    in: header\n    parameter_name:\
  \ session-token\n    role: reusable-parameter\n    description: >-\n      Declared as a reusable header parameter in components.parameters but not\n      referenced by any published operation. Implies a session-based auth mode\n      alongside the bearer JWT.\n    sources:\n      - openapi/tapcart-client-api-openapi-original.json\ninteractive:\n  - surface: Tapcart CLI + MCP server\n    mechanism: Auth0 browser login\n    command: tapcart auth login\n    credential_store: ~/.tapcart/auth.json\n    plan_gate: Tapcart Enterprise plan required for CLI / custom block access.\n    app_id_source: https://app.tapcart.com/settings (Tapcart CLI API Key section)\n    sources:\n      - https://dev.tapcart.com/docs/tapcart-cli\n      - https://dev.tapcart.com/docs/mcp\nauthorization_model:\n  granularity: read vs write\n  description: >-\n    Operation descriptions in the Development API distinguish \"Requires read\n    auth\" from \"Requires write auth\", but the spec expresses both with the same\n\
  \    global bearerAuth requirement and defines no scopes. The read/write split\n    is documented in prose only and is not machine-readable.\ngaps:\n  - No OAuth 2.0 / OIDC machine-to-machine flow is documented for any surface.\n  - No scope or permission reference page exists.\n  - >-\n    The read/write distinction is prose-only; per-operation security\n    requirements in the OpenAPI do not differentiate it.\n  - >-\n    Insights API keys are issued by support, not self-service, so an agent\n    cannot obtain a credential without a human loop.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/authentication/tapcart-authentication.yml
summary_line: http/apiKey · 5 schemes
tags:
- Company
- Mobile
- Commerce
- Shopify
- Ecommerce
- Mobile Apps
- Push Notifications
- Analytics
- Webhooks
- Developer Tools
---
