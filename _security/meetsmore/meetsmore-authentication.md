---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Meetsmore Authentication
name_suffix: Authentication
oauth_flows: []
overview: MeetsMore declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: MeetsMore
provider_slug: meetsmore
scheme_count: 0
schemes: []
slug: meetsmore-authentication
source_filename: meetsmore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: >-\n  https://github.com/meetsmore/nittei — README \"Overview\", crates/api/src/lib.rs\n  (utoipa SecurityAddon), crates/api/src/error.rs and examples/jwt.md — fetched 2026-08-25.\n  derive-authentication.py was not run: there is no openapi/ document in this repository to\n  derive from, because Nittei's OpenAPI is generated at runtime by a self-hosted instance.\nnote: >-\n  The MeetsMore marketplace itself publishes no authentication documentation — its backend\n  (api.meetsmore.com) is a closed AWS API Gateway returning 403 \"Missing Authentication\n  Token\" to anonymous callers, with no public developer program, key issuance or docs.\n  Everything below describes the Nittei Scheduler API.\napis:\n- api: Nittei Scheduler API\n  security_schemes:\n  - name: api_key\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    audience: server-to-server\n    description: >-\n      The account's secret API key. Registered\
  \ in the generated OpenAPI document by\n      utoipa's SecurityAddon as ApiKey::Header(\"x-api-key\"). Used for every admin-scope\n      operation (the *_admin_controller variants). The header name is declared in code as\n      NITTEI_X_API_KEY_HEADER and is added to the Axum SetSensitiveHeadersLayer alongside\n      Authorization so it is redacted from request logs.\n    source: https://github.com/meetsmore/nittei/blob/master/crates/api/src/lib.rs\n  - name: jwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    audience: end-user / browser\n    algorithms:\n    - RS256\n    description: >-\n      For browser-to-server calls. The integrating application uploads its RSA public\n      signing key once via account.setPublicSigningKey (POST set_account_pub_key), then\n      mints a per-user token signed with its private key. RS256 is the only algorithm\n      supported. Claims observed in the published example: nitteiUserId (subject), exp,\n      iat and schedulerPolicy — an\
  \ allow/reject list drawn from a Permissions enum,\n      e.g. allow [Permissions.All], reject [Permissions.DeleteCalendar].\n    source: https://github.com/meetsmore/nittei/blob/master/examples/jwt.md\n  - name: nittei-account\n    type: apiKey\n    in: header\n    parameter: nittei-account\n    audience: end-user / browser\n    description: >-\n      Tenant selector that accompanies the JWT. The API returns 401 with\n      \"Unidentifiable client. Must include the `nittei-account` header\" when it is\n      missing (NitteiError::UnidentifiableClient in crates/api/src/error.rs).\n    source: https://github.com/meetsmore/nittei/blob/master/crates/api/src/error.rs\n  authorization_model:\n    tenancy: >-\n      Account is the multi-tenancy boundary; a User belongs to exactly one Account.\n      Admin operations are authenticated by the account API key; end-user operations are\n      scoped to the user identified in the JWT.\n    permissions: >-\n      Per-token allow/reject policy (schedulerPolicy)\
  \ rather than OAuth scopes. No OAuth\n      scope registry is published, so no scopes/ artifact is emitted for this provider.\n  outbound_oauth:\n    description: >-\n      Nittei acts as an OAuth2 client to connect external calendars. Google and Outlook\n      credentials are exchanged through user::oauth_integration_controller and\n      account::add_account_integration; see IntegrationProvider,\n      OAuthIntegrationRequestBody and OAuthOutlookRequestBody in the generated client types.\n    providers:\n    - Google\n    - Outlook\n- api: use-ai Server\n  security_schemes:\n  - name: none-by-default\n    type: none\n    description: >-\n      use-ai-server ships with no authentication of its own; the README's rationale is\n      that client-side tools \"can already\" be invoked by the browser application, so the\n      MCP bridge adds no privilege. Authorization for anything the server calls onward is\n      forwarded from the client: forwardedPropsProvider supplies an mcpHeaders map\
  \ keyed\n      by picomatch URL patterns, and the server attaches the matching headers only when it\n      calls a remote MCP endpoint whose URL matches.\n    source: https://github.com/meetsmore/use-ai#external-mcps\n  provider_credentials:\n    description: >-\n      Model provider keys are server-side environment variables (e.g. ANTHROPIC_API_KEY),\n      never sent from the browser.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meetsmore/refs/heads/main/authentication/meetsmore-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Marketplace
- Local Services
- Home Services
- Japan
- Scheduling
- Calendar
- Booking
- Field Service
- Open-Source
- Artificial Intelligence
- Agents
---
