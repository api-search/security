---
api_key_in:
- header
auth_types:
- http
- oauth2
description: 'Embrace runs two parallel credential systems. Org-wide API Tokens (auto-created, one capability each: symbol upload, metrics pull, and similar) authenticate the Metrics and Custom Metrics APIs. Service-account bearer tokens (admin-issued, multi-scope, app-scoped, individually revocable) plus an OAuth 2.0 authorization-code flow with PKCE authenticate the MCP server. Both are sent as HTTP Bearer credentials in the Authorization header. There is no OpenAPI document to derive securitySchemes from, so this profile is read from the provider''s own auth documentation and corroborated against the live RFC 8414 / RFC 9728 discovery documents.'
kind: authentication
layout: security
method: searched
name: Embrace Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Embrace secures its APIs with http and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Embrace
provider_slug: embrace
scheme_count: 5
schemes:
- applies_to:
  - embrace-metrics-api
  docs: https://embrace.io/docs/metrics-forwarding/metrics-api/
  format: Bearer <metrics api token>
  in: header
  issued_from: Embrace dashboard → Settings → Organization → API → "Metrics API" token
  name: MetricsApiToken
  parameter: Authorization
  rotation: Replace the whole org token.
  scheme: bearer
  scope_of_access: entire organization
  type: http
- applies_to:
  - embrace-custom-metrics-api
  docs: https://embrace.io/docs/metrics-forwarding/custom-metrics/custom-metrics-api/
  format: Bearer <custom metrics api token>
  in: header
  issued_from: Issued on request by an Embrace onboarding specialist. This is explicitly a different token than the Metrics API token, and it is not self-service — a sales/onboarding gate sits in front of the Custom Metrics API even though the reference documentation is public.
  name: CustomMetricsApiToken
  parameter: Authorization
  scheme: bearer
  type: http
- applies_to:
  - build-tooling
  detail: Consumed by embrace-web-cli (-t flag), the iOS Run Script dSYM upload phase, the Android Gradle plugin and the embrace-io/action-symbol-upload GitHub Action. Paired with the 5-character Embrace App ID, which is an identifier rather than a secret.
  docs: https://embrace.io/docs/web/getting-started/sourcemap-uploads/
  in: header
  issued_from: Embrace dashboard → Settings → API
  name: SymbolUploadToken
  parameter: Authorization
  scheme: bearer
  type: http
- app_scoping: All apps in the org (including future apps) or an explicit app list.
  applies_to:
  - embrace-mcp-server
  docs: https://embrace.io/docs/product/settings/service-accounts/
  format: Bearer emb_sa_<43 characters>  (50 characters total)
  identity_in_logs: Named service account, e.g. "Service account 'CI Pipeline' did X".
  in: header
  issued_from: Settings → Organization → API → Service Accounts (org admins only)
  name: ServiceAccountBearerToken
  parameter: Authorization
  prefix: emb_sa_
  rotation: A service account can hold several live tokens, so rotation is create-new → deploy → confirm the Last used timestamp updates → revoke old. Revocation is immediate; deleting the service account revokes all of its tokens.
  scheme: bearer
  scopes:
  - mcp:tools:call
  - mcp:read
  - mcp:write
  shown_once: true
  type: http
- applies_to:
  - embrace-mcp-server
  detail: The MCP server advertises RFC 9728 protected-resource metadata pointing at the dash-api.embrace.io authorization server, which in turn advertises RFC 8414 metadata with a dynamic client registration endpoint. Tokens issued through this flow are tied to the individual Embrace user and inherit that user's app permissions.
  docs: https://embrace.io/docs/mcp/
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://dash.embrace.io/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    issuer: https://dash-api.embrace.io
    jwksUri: https://dash-api.embrace.io/.well-known/jwks.json
    pkce_methods:
    - S256
    registrationUrl: https://dash-api.embrace.io/oauth/register
    revocationUrl: https://dash-api.embrace.io/oauth/revoke
    scopes:
    - mcp:read
    - mcp:write
    - mcp:tools:call
    tokenUrl: https://dash-api.embrace.io/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_basic
    - client_secret_post
  name: EmbraceMcpOAuth2
  type: oauth2
slug: embrace-authentication
source_filename: embrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://embrace.io/docs/product/settings/service-accounts/\ndocs:\n  - https://embrace.io/docs/product/settings/api-tokens/\n  - https://embrace.io/docs/product/settings/service-accounts/\n  - https://embrace.io/docs/mcp/\n  - https://embrace.io/docs/metrics-forwarding/metrics-api/\n  - https://embrace.io/docs/metrics-forwarding/custom-metrics/custom-metrics-api/\nprobe:\n  - {url: 'https://mcp.embrace.io/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://mcp.embrace.io/.well-known/oauth-protected-resource', status: 200}\n  - {url: 'https://dash-api.embrace.io/.well-known/jwks.json', status: 200}\ndescription: >-\n  Embrace runs two parallel credential systems. Org-wide API Tokens (auto-created, one capability\n  each: symbol upload, metrics pull, and similar) authenticate the Metrics and Custom Metrics\n  APIs. Service-account bearer tokens (admin-issued, multi-scope, app-scoped, individually\n  revocable)\
  \ plus an OAuth 2.0 authorization-code flow with PKCE authenticate the MCP server.\n  Both are sent as HTTP Bearer credentials in the Authorization header. There is no OpenAPI\n  document to derive securitySchemes from, so this profile is read from the provider's own auth\n  documentation and corroborated against the live RFC 8414 / RFC 9728 discovery documents.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\nschemes:\n  - name: MetricsApiToken\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: \"Bearer <metrics api token>\"\n    applies_to: [embrace-metrics-api]\n    issued_from: Embrace dashboard → Settings → Organization → API → \"Metrics API\" token\n    scope_of_access: entire organization\n    rotation: Replace the whole org token.\n    docs: https://embrace.io/docs/metrics-forwarding/metrics-api/\n  - name: CustomMetricsApiToken\n    type: http\n \
  \   scheme: bearer\n    in: header\n    parameter: Authorization\n    format: \"Bearer <custom metrics api token>\"\n    applies_to: [embrace-custom-metrics-api]\n    issued_from: >-\n      Issued on request by an Embrace onboarding specialist. This is explicitly a different token\n      than the Metrics API token, and it is not self-service — a sales/onboarding gate sits in\n      front of the Custom Metrics API even though the reference documentation is public.\n    docs: https://embrace.io/docs/metrics-forwarding/custom-metrics/custom-metrics-api/\n  - name: SymbolUploadToken\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    applies_to: [build-tooling]\n    issued_from: Embrace dashboard → Settings → API\n    detail: >-\n      Consumed by embrace-web-cli (-t flag), the iOS Run Script dSYM upload phase, the Android\n      Gradle plugin and the embrace-io/action-symbol-upload GitHub Action. Paired with the\n      5-character Embrace App ID, which is\
  \ an identifier rather than a secret.\n    docs: https://embrace.io/docs/web/getting-started/sourcemap-uploads/\n  - name: ServiceAccountBearerToken\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: \"Bearer emb_sa_<43 characters>  (50 characters total)\"\n    prefix: emb_sa_\n    applies_to: [embrace-mcp-server]\n    issued_from: Settings → Organization → API → Service Accounts (org admins only)\n    scopes: [mcp:tools:call, mcp:read, mcp:write]\n    app_scoping: All apps in the org (including future apps) or an explicit app list.\n    identity_in_logs: Named service account, e.g. \"Service account 'CI Pipeline' did X\".\n    shown_once: true\n    rotation: >-\n      A service account can hold several live tokens, so rotation is create-new → deploy →\n      confirm the Last used timestamp updates → revoke old. Revocation is immediate; deleting the\n      service account revokes all of its tokens.\n    docs: https://embrace.io/docs/product/settings/service-accounts/\n\
  \  - name: EmbraceMcpOAuth2\n    type: oauth2\n    applies_to: [embrace-mcp-server]\n    flows:\n      - flow: authorizationCode\n        issuer: https://dash-api.embrace.io\n        authorizationUrl: https://dash.embrace.io/oauth/authorize\n        tokenUrl: https://dash-api.embrace.io/oauth/token\n        registrationUrl: https://dash-api.embrace.io/oauth/register\n        revocationUrl: https://dash-api.embrace.io/oauth/revoke\n        jwksUri: https://dash-api.embrace.io/.well-known/jwks.json\n        scopes: [mcp:read, mcp:write, mcp:tools:call]\n        grant_types: [authorization_code, refresh_token]\n        pkce_methods: [S256]\n        token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    dynamic_client_registration: true    # RFC 7591 registration_endpoint advertised\n    detail: >-\n      The MCP server advertises RFC 9728 protected-resource metadata pointing at the\n      dash-api.embrace.io authorization server, which in turn advertises RFC 8414\
  \ metadata with a\n      dynamic client registration endpoint. Tokens issued through this flow are tied to the\n      individual Embrace user and inherit that user's app permissions.\n    docs: https://embrace.io/docs/mcp/\ngaps:\n  - >-\n    No OpenAPI/Swagger document is published for the Metrics or Custom Metrics APIs, so there are\n    no machine-readable securitySchemes to validate this profile against.\n  - >-\n    api.embrace.io returns 403 to every anonymous request including /.well-known/*, so the REST\n    auth surface cannot be confirmed by probe — only by documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embrace/refs/heads/main/authentication/embrace-authentication.yml
summary_line: http/oauth2 · 5 schemes
tags:
- Company
- Observability
- Monitoring
- Mobile
- Real User Monitoring
- OpenTelemetry
- Metrics
- Crash Reporting
- Application Performance Monitoring
- Developer Tools
- Model Context Protocol
---
