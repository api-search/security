---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Funnel Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Funnel secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Funnel
provider_slug: funnel
scheme_count: 3
schemes:
- additional_requirement:
    detail: A valid token is NOT sufficient. The Control Plane API rejects any request whose User-Agent is not "terraform-provider-funnel" with HTTP 400 before authentication is even evaluated, and rejects a version below its advertised minimum (currently 0.1.0) the same way. Verified live on 2026-08-12. This is an undocumented client-lock-in gate; see conventions/funnel-conventions.yml.
    header: User-Agent
    value: terraform-provider-funnel/<version>
  api: Funnel Control Plane API
  audience:
  - https://controlplane.setup.us.funnel.io
  - https://controlplane.setup.eu.funnel.io
  credentials:
  - client_id
  - client_secret
  description: Server-to-server OAuth 2.0 client-credentials flow. A "System user" is created per subscription in the Funnel app (Subscription overview -> Authentication), yielding a client_id and client_secret. These are exchanged at the Auth0 token endpoint with the region-appropriate audience for a Bearer access token used against the regional Control Plane API host.
  flow: clientCredentials
  grant_type: client_credentials
  identity_provider: Auth0
  name: FunnelSystemUserOAuth
  scopes: []
  sources:
  - registry.terraform.io/providers/funnel-io/funnel/latest/docs
  - provider/auth/auth0_client.go
  token_type: Bearer
  token_url: https://login.funnel.io/oauth/token
  token_url_eu: https://login.funnel.io/oauth/token
  type: oauth2
- api: Funnel MCP
  authorization_server: https://login.funnel.io
  description: Interactive, user-delegated OAuth 2.0 authorization-code flow. The MCP client is registered dynamically at https://login.funnel.io/oidc/register (or given a static client ID copied from Funnel AI > MCP > Advanced for clients that cannot do DCR), the end user signs in to Funnel in a browser, and the resulting Bearer token authorizes read-only tool calls scoped to that user's own workspace permissions. Missing or absent tokens return a JSON-RPC error {"code":-32001,"message":"Missing Bearer token"} with HTTP 401.
  dynamic_client_registration: true
  flow: authorizationCode
  known_failure_modes:
  - Dynamic client registration failing in Claude Desktop via mcp-remote.
  - OAuth callback URL mismatch on login.funnel.io.
  - token_exchange_failed after OAuth appears to succeed.
  - '"Unknown client" invalid_request when connecting from Notion.'
  known_failure_modes_source: https://help.funnel.io/en/collections/19637543-funnel-mcp
  name: FunnelMCPOAuth
  protected_resource_metadata:
  - well-known/funnel-mcp-oauth-protected-resource.json
  - well-known/funnel-mcp-eu-oauth-protected-resource.json
  resource:
  - https://mcp.ai.funnel.io/mcp
  - https://mcp.eu.ai.funnel.io/mcp
  rfc: RFC 9728 (OAuth 2.0 Protected Resource Metadata)
  scopes:
  - openid
  - profile
  - email
  - offline_access
  see: scopes/funnel-scopes.yml
  static_client_id_available: true
  token_type: Bearer
  type: oauth2
- api: Funnel File Import Webhook API
  description: Static secret token generated per File Import data source inside the Funnel app when the Webhook transport type is enabled. Paired with a per-source webhook URL of the form https://fileimport-webhook.funnel.io/{webhook_id}. Requests without a matching token are denied with HTTP 401 "Invalid credentials". No rotation policy, expiry or signature scheme is published.
  in: header
  name: x-funnel-fileimport-token
  scope: per-data-source
  type: apiKey
slug: funnel-authentication
source_filename: funnel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://registry.terraform.io/providers/funnel-io/funnel/latest/docs +\n  provider/auth/auth0_client.go (github.com/funnel-io/terraform-provider-funnel) +\n  https://login.funnel.io/.well-known/openid-configuration +\n  https://mcp.ai.funnel.io/.well-known/oauth-protected-resource/mcp +\n  https://help.funnel.io/en/articles/15014203-quick-start-guide-using-funnel-mcp +\n  https://help.funnel.io/en/articles/8439795-file-import-webhook-api-documentation\ndocs: https://registry.terraform.io/providers/funnel-io/funnel/latest/docs\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - apiKey\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  api_key_in:\n  - header\nauthorization_server:\n  issuer: https://login.funnel.io/\n  identity_provider: Auth0\n  discovery: https://login.funnel.io/.well-known/openid-configuration\n  discovery_http_status: 200\n  discovery_file: well-known/funnel-login-openid-configuration.json\n\
  \  token_endpoint: https://login.funnel.io/oauth/token\n  authorization_endpoint: https://login.funnel.io/authorize\n  registration_endpoint: https://login.funnel.io/oidc/register\n  dynamic_client_registration: true\n  pkce_methods:\n  - S256\n  - plain\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  detail: >-\n    One Auth0 tenant on Funnel's own domain fronts every programmatic surface. It serves a real OIDC\n    discovery document anonymously and advertises RFC 7591 dynamic client registration, which is what\n    lets MCP clients such as Claude register themselves without a pre-shared client ID.\nschemes:\n- name: FunnelSystemUserOAuth\n  api: Funnel Control Plane API\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://login.funnel.io/oauth/token\n  token_url_eu: https://login.funnel.io/oauth/token\n  identity_provider: Auth0\n  audience:\n  - https://controlplane.setup.us.funnel.io\n  - https://controlplane.setup.eu.funnel.io\n\
  \  grant_type: client_credentials\n  token_type: Bearer\n  credentials:\n  - client_id\n  - client_secret\n  scopes: []\n  sources:\n  - registry.terraform.io/providers/funnel-io/funnel/latest/docs\n  - provider/auth/auth0_client.go\n  description: >-\n    Server-to-server OAuth 2.0 client-credentials flow. A \"System user\" is created per subscription\n    in the Funnel app (Subscription overview -> Authentication), yielding a client_id and\n    client_secret. These are exchanged at the Auth0 token endpoint with the region-appropriate\n    audience for a Bearer access token used against the regional Control Plane API host.\n  additional_requirement:\n    header: User-Agent\n    value: terraform-provider-funnel/<version>\n    detail: >-\n      A valid token is NOT sufficient. The Control Plane API rejects any request whose User-Agent is\n      not \"terraform-provider-funnel\" with HTTP 400 before authentication is even evaluated, and\n      rejects a version below its advertised minimum\
  \ (currently 0.1.0) the same way. Verified live\n      on 2026-08-12. This is an undocumented client-lock-in gate; see\n      conventions/funnel-conventions.yml.\n- name: FunnelMCPOAuth\n  api: Funnel MCP\n  type: oauth2\n  flow: authorizationCode\n  authorization_server: https://login.funnel.io\n  resource:\n  - https://mcp.ai.funnel.io/mcp\n  - https://mcp.eu.ai.funnel.io/mcp\n  protected_resource_metadata:\n  - well-known/funnel-mcp-oauth-protected-resource.json\n  - well-known/funnel-mcp-eu-oauth-protected-resource.json\n  rfc: RFC 9728 (OAuth 2.0 Protected Resource Metadata)\n  token_type: Bearer\n  dynamic_client_registration: true\n  static_client_id_available: true\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  see: scopes/funnel-scopes.yml\n  description: >-\n    Interactive, user-delegated OAuth 2.0 authorization-code flow. The MCP client is registered\n    dynamically at https://login.funnel.io/oidc/register (or given a static client ID copied from\n \
  \   Funnel AI > MCP > Advanced for clients that cannot do DCR), the end user signs in to Funnel in a\n    browser, and the resulting Bearer token authorizes read-only tool calls scoped to that user's own\n    workspace permissions. Missing or absent tokens return a JSON-RPC error\n    {\"code\":-32001,\"message\":\"Missing Bearer token\"} with HTTP 401.\n  known_failure_modes:\n  - Dynamic client registration failing in Claude Desktop via mcp-remote.\n  - OAuth callback URL mismatch on login.funnel.io.\n  - token_exchange_failed after OAuth appears to succeed.\n  - '\"Unknown client\" invalid_request when connecting from Notion.'\n  known_failure_modes_source: https://help.funnel.io/en/collections/19637543-funnel-mcp\n- name: FunnelFileImportToken\n  api: Funnel File Import Webhook API\n  type: apiKey\n  in: header\n  name: x-funnel-fileimport-token\n  scope: per-data-source\n  description: >-\n    Static secret token generated per File Import data source inside the Funnel app when the\
  \ Webhook\n    transport type is enabled. Paired with a per-source webhook URL of the form\n    https://fileimport-webhook.funnel.io/{webhook_id}. Requests without a matching token are denied\n    with HTTP 401 \"Invalid credentials\". No rotation policy, expiry or signature scheme is published.\nenterprise_sso:\n  available_on: Enterprise plan only\n  methods:\n  - SAML\n  - OIDC\n  - SCIM\n  - Sign-in with Google\n  identity_providers_named:\n  - Okta\n  - Azure AD\n  source: https://funnel.io/pricing\n  detail: >-\n    End-user (human) authentication into the Funnel app. Gated to the Enterprise tier; Starter and\n    Business get Sign-in with Google only.\nnotes: >-\n  Three distinct authentication schemes across three distinct programmatic surfaces, all anchored on\n  one Auth0 tenant at login.funnel.io. Scopes exist only on the MCP surface and are identity scopes,\n  not resource scopes — the Control Plane grant is authorized by audience and scoped by\n  subscription_id instead. Authentication\
  \ is region-aware throughout: US and EU use distinct Control\n  Plane hosts and audiences, and distinct MCP hosts, for data residency.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funnel/refs/heads/main/authentication/funnel-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Marketing
- Marketing Intelligence
- Marketing Data
- Analytics
- Advertising
- Data Integration
- ETL
- Data Warehouse
- Attribution
- Reporting
- Business Intelligence
- MCP
- AI Agents
- Marketing Mix Modeling
---
