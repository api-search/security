---
api_key_in:
- header
api_specs:
- filename: hightouch-api-openapi.json
  format: json
  label: Hightouch API
  slug: hightouch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/_original/hightouch-api-openapi.json
- filename: hightouch-sources-api-openapi.yml
  format: yaml
  label: Hightouch Sources API
  slug: hightouch-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-sources-api-openapi.yml
- filename: hightouch-models-api-openapi.yml
  format: yaml
  label: Hightouch Models API
  slug: hightouch-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-models-api-openapi.yml
- filename: hightouch-destinations-api-openapi.yml
  format: yaml
  label: Hightouch Destinations API
  slug: hightouch-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-destinations-api-openapi.yml
- filename: hightouch-syncs-api-openapi.yml
  format: yaml
  label: Hightouch Syncs API
  slug: hightouch-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-syncs-api-openapi.yml
- filename: hightouch-campaigns-api-openapi.yml
  format: yaml
  label: Hightouch Campaigns API
  slug: hightouch-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-campaigns-api-openapi.yml
- filename: hightouch-ai-decisioning-api-openapi.yml
  format: yaml
  label: Hightouch AI Decisioning API
  slug: hightouch-ai-decisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-ai-decisioning-api-openapi.yml
- filename: hightouch-events-api-openapi.yml
  format: yaml
  label: Hightouch Events API
  slug: hightouch-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-events-api-openapi.yml
- filename: hightouch-identity-resolution-api-openapi.yml
  format: yaml
  label: Hightouch Identity Resolution API
  slug: hightouch-identity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-identity-resolution-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hightouch Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hightouch secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hightouch
provider_slug: hightouch
scheme_count: 3
schemes:
- applies_to: https://api.hightouch.com/api/v1 (all 43 operations)
  bearerFormat: Bearer
  credential: Workspace API key created by an Admin user under Settings > API keys
  env_var: HIGHTOUCH_APIKEY (used by the ht CLI)
  name: bearerAuth
  notes:
  - Keys authenticate AS THEIR CREATING USER. If that user is deactivated, loses workspace access, or is removed during an SSO migration, every key they created stops working — the provider documents this as the most common cause of 401s.
  - Admin role is required to create an API key.
  - TLS 1.2 or later is required; the API publishes its accepted cipher suite list.
  - Keys are revocable individually from the Settings > API keys tab.
  scheme: bearer
  sources:
  - openapi/_original/hightouch-api-openapi.json
  type: http
- applies_to: https://api.hightouch.com/api/v1/a2a/messages and the workspace MCP server
  flows:
  - authorizationUrl: https://mcp-auth.hightouch.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://mcp-auth.hightouch.com/oauth2/token
  name: oauth2
  notes:
  - 'Protected-resource metadata is advertised per RFC 9728; an unauthenticated POST to the A2A endpoint returns 401 with WWW-Authenticate: Bearer resource_metadata="https://api.hightouch.com/.well-known/oauth-protected-resource".'
  - Dynamic client registration is open at /oauth2/register.
  - token_endpoint_auth_methods_supported includes `none`, i.e. public PKCE clients are allowed.
  scopes:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - a2a/hightouch-agent-card.json
  - https://api.hightouch.com/.well-known/oauth-authorization-server
  type: oauth2
- name: openIdConnect
  notes:
  - Same issuer as the OAuth AS (mcp-auth.hightouch.com); RS256 ID tokens; userinfo endpoint.
  openIdConnectUrl: https://api.hightouch.com/.well-known/openid-configuration
  sources:
  - well-known/hightouch-openid-configuration.json
  type: openIdConnect
slug: hightouch-authentication
source_filename: hightouch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/hightouch-api-openapi.json, https://hightouch.com/docs/developer-tools/api-guide,\n  https://api.hightouch.com/.well-known/oauth-protected-resource, a2a/hightouch-agent-card.json\ndocs: https://hightouch.com/docs/developer-tools/api-guide\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  surfaces:\n    rest_management_api: bearer workspace API key\n    a2a_agent: oauth2 authorizationCode (mcp-auth.hightouch.com)\n    workspace_mcp: oauth2 (same authorization server)\n    docs_mcp: none (anonymous)\n    events_ingest: write key (per-source), see https://hightouch.com/docs/events/overview\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer\n  sources:\n  - openapi/_original/hightouch-api-openapi.json\n  applies_to: https://api.hightouch.com/api/v1 (all 43 operations)\n  credential: Workspace API\
  \ key created by an Admin user under Settings > API keys\n  env_var: HIGHTOUCH_APIKEY (used by the ht CLI)\n  notes:\n  - Keys authenticate AS THEIR CREATING USER. If that user is deactivated, loses workspace access, or\n    is removed during an SSO migration, every key they created stops working — the provider documents\n    this as the most common cause of 401s.\n  - Admin role is required to create an API key.\n  - TLS 1.2 or later is required; the API publishes its accepted cipher suite list.\n  - Keys are revocable individually from the Settings > API keys tab.\n- name: oauth2\n  type: oauth2\n  sources:\n  - a2a/hightouch-agent-card.json\n  - https://api.hightouch.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp-auth.hightouch.com/oauth2/authorize\n    tokenUrl: https://mcp-auth.hightouch.com/oauth2/token\n  applies_to: https://api.hightouch.com/api/v1/a2a/messages and the workspace MCP server\n  scopes:\n  - openid\n\
  \  - profile\n  - email\n  - offline_access\n  notes:\n  - 'Protected-resource metadata is advertised per RFC 9728; an unauthenticated POST to the A2A endpoint\n    returns 401 with WWW-Authenticate: Bearer resource_metadata=\"https://api.hightouch.com/.well-known/oauth-protected-resource\".'\n  - Dynamic client registration is open at /oauth2/register.\n  - token_endpoint_auth_methods_supported includes `none`, i.e. public PKCE clients are allowed.\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.hightouch.com/.well-known/openid-configuration\n  sources:\n  - well-known/hightouch-openid-configuration.json\n  notes:\n  - Same issuer as the OAuth AS (mcp-auth.hightouch.com); RS256 ID tokens; userinfo endpoint.\nworkspace_access_control:\n  sso: SAML 2.0 / Okta / Azure AD / Google — https://hightouch.com/docs/workspace-management/sso\n  rbac: https://hightouch.com/docs/workspace-management/roles\n  approval_flows: https://hightouch.com/docs/workspace-management/approval-flows\n\
  \  audit_logs: https://hightouch.com/docs/workspace-management/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/authentication/hightouch-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- CDP
- Data Activation
- Reverse ETL
- Audience Management
- Identity Resolution
- Event Collection
- Marketing
- Advertising
- AI Agents
- Data Warehouse
---
