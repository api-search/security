---
anonymous_access: false
api_key_in: []
api_specs:
- filename: betterstack-heartbeats-api-openapi.yml
  format: yaml
  label: Better Stack Heartbeats API
  slug: betterstack-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/openapi/betterstack-heartbeats-api-openapi.yml
- filename: betterstack-incidents-api-openapi.yml
  format: yaml
  label: Better Stack Incidents API
  slug: betterstack-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/openapi/betterstack-incidents-api-openapi.yml
- filename: betterstack-monitors-api-openapi.yml
  format: yaml
  label: Better Stack Monitors API
  slug: betterstack-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/openapi/betterstack-monitors-api-openapi.yml
- filename: betterstack-status-pages-api-openapi.yml
  format: yaml
  label: Better Stack Status Pages API
  slug: betterstack-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/openapi/betterstack-status-pages-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Betterstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Better Stack secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Better Stack
provider_slug: betterstack
scheme_count: 3
schemes:
- description: 'Static bearer token sent as `Authorization: Bearer $TOKEN`. Better Stack calls this "the Bearer Authentication standard". This is the only credential the REST APIs accept.'
  expiry_documented: false
  name: bearerAuth
  rotation_documented: false
  scheme: bearer
  scope_note: Tokens carry no OAuth scopes. The only narrowing available is choosing a team-scoped token over a global one; within its team a token is unrestricted read AND write.
  scoped: false
  sources:
  - https://betterstack.com/docs/uptime/api/getting-started-with-uptime-api/
  - openapi/betterstack-monitors-api-openapi.yml
  surface: REST — Uptime v2, Telemetry v1, Errors v1
  token_types:
  - issued_at: Better Stack → API tokens → Global API tokens
    name: Global API token
    scope: All teams in the organization; manages anything in Better Stack.
  - issued_at: Better Stack → API tokens → Team-based tokens → Uptime API tokens
    name: Uptime API token
    scope: One team's Uptime resources.
  - issued_at: Better Stack → API tokens → Team-based tokens
    name: Telemetry API token
    scope: One team's Telemetry resources; also accepted by the Errors API.
  type: http
- description: 'A per-source ingestion token sent as `Authorization: Bearer $SOURCE_TOKEN` when posting OTLP/HTTP to $INGESTING_HOST/v1/logs, /v1/traces and /v1/metrics. Distinct from the management API tokens above — it writes telemetry in, it does not read or manage anything.'
  name: sourceToken
  scheme: bearer
  sources:
  - https://betterstack.com/docs/logs/open-telemetry/
  surface: OTLP ingestion
  type: http
- description: OAuth 2.1 authorization-code flow with PKCE and dynamic client registration, used by the Better Stack MCP server. Not available on the REST APIs.
  discovery:
  - https://betterstack.com/.well-known/oauth-authorization-server
  - https://mcp.betterstack.com/.well-known/oauth-protected-resource
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://betterstack.com/oauth/authorize
      refreshUrl: https://betterstack.com/oauth/token
      registrationUrl: https://betterstack.com/oauth/register
      scopes:
        read: Read access to Better Stack resources.
        write: Write access to Better Stack resources.
      tokenUrl: https://betterstack.com/oauth/token
  name: oauth2
  note: The MCP server also accepts a static Better Stack API token as a bearer credential for clients that cannot do OAuth.
  pkce: S256
  sources:
  - well-known/betterstack-oauth-authorization-server.json
  - well-known/betterstack-mcp-oauth-protected-resource.json
  - https://betterstack.com/docs/getting-started/integrations/mcp/
  surface: MCP server (https://mcp.betterstack.com)
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: betterstack-authentication
source_filename: betterstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://betterstack.com/docs/uptime/api/getting-started-with-uptime-api/,\n  https://betterstack.com/docs/logs/api/getting-started/,\n  https://betterstack.com/docs/errors/api/,\n  https://betterstack.com/docs/getting-started/integrations/mcp/,\n  https://betterstack.com/docs/logs/open-telemetry/, the RFC 8414 and RFC 9728 discovery\n  documents saved under well-known/, and live unauthenticated probes on 2026-09-04. Upgraded\n  from the derived profile that read only the bearerAuth scheme out of openapi/.\ndocs: https://betterstack.com/docs/uptime/api/getting-started-with-uptime-api/\nprovider: Better Stack\nproviderId: betterstack\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: REST — Uptime v2, Telemetry v1, Errors v1\n  description: >-\n    Static bearer token sent as `Authorization: Bearer $TOKEN`. Better Stack calls this \"the\n    Bearer Authentication\
  \ standard\". This is the only credential the REST APIs accept.\n  token_types:\n  - name: Global API token\n    scope: All teams in the organization; manages anything in Better Stack.\n    issued_at: Better Stack → API tokens → Global API tokens\n  - name: Uptime API token\n    scope: One team's Uptime resources.\n    issued_at: Better Stack → API tokens → Team-based tokens → Uptime API tokens\n  - name: Telemetry API token\n    scope: One team's Telemetry resources; also accepted by the Errors API.\n    issued_at: Better Stack → API tokens → Team-based tokens\n  scoped: false\n  scope_note: >-\n    Tokens carry no OAuth scopes. The only narrowing available is choosing a team-scoped token\n    over a global one; within its team a token is unrestricted read AND write.\n  rotation_documented: false\n  expiry_documented: false\n  sources:\n  - https://betterstack.com/docs/uptime/api/getting-started-with-uptime-api/\n  - openapi/betterstack-monitors-api-openapi.yml\n- name: sourceToken\n\
  \  type: http\n  scheme: bearer\n  surface: OTLP ingestion\n  description: >-\n    A per-source ingestion token sent as `Authorization: Bearer $SOURCE_TOKEN` when posting\n    OTLP/HTTP to $INGESTING_HOST/v1/logs, /v1/traces and /v1/metrics. Distinct from the\n    management API tokens above — it writes telemetry in, it does not read or manage anything.\n  sources:\n  - https://betterstack.com/docs/logs/open-telemetry/\n- name: oauth2\n  type: oauth2\n  surface: MCP server (https://mcp.betterstack.com)\n  description: >-\n    OAuth 2.1 authorization-code flow with PKCE and dynamic client registration, used by the\n    Better Stack MCP server. Not available on the REST APIs.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://betterstack.com/oauth/authorize\n      tokenUrl: https://betterstack.com/oauth/token\n      registrationUrl: https://betterstack.com/oauth/register\n      refreshUrl: https://betterstack.com/oauth/token\n      scopes:\n        read: Read access to Better\
  \ Stack resources.\n        write: Write access to Better Stack resources.\n  pkce: S256\n  dynamic_client_registration: true\n  token_endpoint_auth_methods_supported: [none]\n  discovery:\n  - https://betterstack.com/.well-known/oauth-authorization-server\n  - https://mcp.betterstack.com/.well-known/oauth-protected-resource\n  sources:\n  - well-known/betterstack-oauth-authorization-server.json\n  - well-known/betterstack-mcp-oauth-protected-resource.json\n  - https://betterstack.com/docs/getting-started/integrations/mcp/\n  note: >-\n    The MCP server also accepts a static Better Stack API token as a bearer credential for\n    clients that cannot do OAuth.\nsso:\n  consumed: true\n  providers: [Okta, Azure AD]\n  note: >-\n    SSO is a paid Enterprise add-on for signing INTO Better Stack ($5 per user/month per the\n    pricing page). Better Stack is an SSO relying party, not an identity provider —\n    /.well-known/openid-configuration 404s on every host.\ngaps:\n- No mTLS, request\
  \ signing or HMAC option on any surface.\n- No documented token rotation policy, expiry, or revocation endpoint for the static REST\n  tokens.\n- The REST tokens carry no scopes, so least-privilege is limited to team boundaries.\n- 401 responses are identical for a missing credential and an invalid one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/authentication/betterstack-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Observability
- Uptime Monitoring
- Incidents
- Logs
- Monitoring
- Status Pages
- On-Call
- Error Tracking
- OpenTelemetry
- Model Context Protocol
---
