---
api_key_in:
- header
api_specs:
- filename: agorapulse-calendar-notes-api-openapi.yml
  format: yaml
  label: Agorapulse Calendar Notes API
  slug: agorapulse-calendar-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-calendar-notes-api-openapi.yml
- filename: agorapulse-agorapulse-api-api-openapi.yml
  format: yaml
  label: Agorapulse Webhooks API
  slug: agorapulse-agorapulse-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-agorapulse-api-api-openapi.yml
- filename: agorapulse-competitor-api-openapi.yml
  format: yaml
  label: Agorapulse Competitor API
  slug: agorapulse-competitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-competitor-api-openapi.yml
- filename: agorapulse-conversations-api-openapi.yml
  format: yaml
  label: Agorapulse Conversations API
  slug: agorapulse-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-conversations-api-openapi.yml
- filename: agorapulse-drafts-api-openapi.yml
  format: yaml
  label: Agorapulse Drafts API
  slug: agorapulse-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-drafts-api-openapi.yml
- filename: agorapulse-groups-api-openapi.yml
  format: yaml
  label: Agorapulse Groups API
  slug: agorapulse-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-groups-api-openapi.yml
- filename: agorapulse-health-api-openapi.yml
  format: yaml
  label: Agorapulse Health API
  slug: agorapulse-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-health-api-openapi.yml
- filename: agorapulse-items-api-openapi.yml
  format: yaml
  label: Agorapulse Items API
  slug: agorapulse-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-items-api-openapi.yml
- filename: agorapulse-media-api-openapi.yml
  format: yaml
  label: Agorapulse Media API
  slug: agorapulse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-media-api-openapi.yml
- filename: agorapulse-organizations-api-openapi.yml
  format: yaml
  label: Agorapulse Organizations API
  slug: agorapulse-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-organizations-api-openapi.yml
- filename: agorapulse-pinterest-boards-api-openapi.yml
  format: yaml
  label: Agorapulse Pinterest boards API
  slug: agorapulse-pinterest-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-pinterest-boards-api-openapi.yml
- filename: agorapulse-profiles-api-openapi.yml
  format: yaml
  label: Agorapulse Profiles API
  slug: agorapulse-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-profiles-api-openapi.yml
- filename: agorapulse-replies-api-openapi.yml
  format: yaml
  label: Agorapulse Replies API
  slug: agorapulse-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-replies-api-openapi.yml
- filename: agorapulse-reports-api-openapi.yml
  format: yaml
  label: Agorapulse Reports API
  slug: agorapulse-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-reports-api-openapi.yml
- filename: agorapulse-workspaces-api-openapi.yml
  format: yaml
  label: Agorapulse Workspaces API
  slug: agorapulse-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-workspaces-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: Agorapulse runs two independent authentication models. The REST API is a single static API key in an X-API-KEY header, scoped to the individual user who minted it. The remote MCP server is a separate OAuth 2.0 protected resource with its own authorization server, dynamic client registration and PKCE. They do not share credentials.
kind: authentication
layout: security
method: searched
name: Agorapulse Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Agorapulse secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Agorapulse
provider_slug: agorapulse
scheme_count: 3
schemes:
- applies_to: All REST operations (declared as the document-level security requirement).
  description: Despite the scheme name, this is not a bearer token — it is a raw API key in an X-API-KEY header. Keys are minted per user at Personal settings -> API Keys and are shown once. Permissions are inherited from the user's own role, so the key of an org owner or manager is needed for full profile coverage. Requests without a valid key return 401.
  in: header
  name: bearerAuth
  parameter: X-API-KEY
  sources:
  - openapi/_original/agorapulse-open-api-openapi.yml
  - https://support.agorapulse.com/en/articles/12417183-how-to-connect-to-agorapulse-s-open-api
  type: apiKey
- applies_to: Inbound webhook deliveries (PUBLISHING_POST, INBOX_ITEM).
  description: SHA256 HMAC of the raw request body, computed with the shared secret from the webhook subscription. Verified by the receiver, not sent by the caller.
  in: header
  name: HookSignature
  parameter: X-Hook-Signature
  sources:
  - openapi/_original/agorapulse-open-api-openapi.yml
  type: apiKey
- applies_to: The remote MCP server at https://api.openmcp.agorapulse.com/mcp
  flows:
  - authorizationUrl: https://api.identity.agorapulse.com/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    registrationUrl: https://api.identity.agorapulse.com/oauth/register
    resource_parameter_supported: true
    scopes:
    - read
    tokenUrl: https://api.identity.agorapulse.com/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
    userinfoUrl: https://api.identity.agorapulse.com/oauth/userinfo
  name: MCP OAuth
  sources:
  - well-known/agorapulse-oauth-authorization-server.json
  - well-known/agorapulse-oauth-protected-resource.json
  type: oauth2
slug: agorapulse-authentication
source_filename: agorapulse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/agorapulse-open-api-openapi.yml\ndocs: https://support.agorapulse.com/en/articles/12417183-how-to-connect-to-agorapulse-s-open-api\ndescription: >-\n  Agorapulse runs two independent authentication models. The REST API is a single static API key in\n  an X-API-KEY header, scoped to the individual user who minted it. The remote MCP server is a\n  separate OAuth 2.0 protected resource with its own authorization server, dynamic client\n  registration and PKCE. They do not share credentials.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  applies_to: All REST operations (declared as the document-level security requirement).\n  description: >-\n    Despite the scheme name, this is not a bearer token — it is a raw API key in an X-API-KEY header.\n    Keys are minted per user at\
  \ Personal settings -> API Keys and are shown once. Permissions are\n    inherited from the user's own role, so the key of an org owner or manager is needed for full\n    profile coverage. Requests without a valid key return 401.\n  sources:\n  - openapi/_original/agorapulse-open-api-openapi.yml\n  - https://support.agorapulse.com/en/articles/12417183-how-to-connect-to-agorapulse-s-open-api\n- name: HookSignature\n  type: apiKey\n  in: header\n  parameter: X-Hook-Signature\n  applies_to: Inbound webhook deliveries (PUBLISHING_POST, INBOX_ITEM).\n  description: >-\n    SHA256 HMAC of the raw request body, computed with the shared secret from the webhook\n    subscription. Verified by the receiver, not sent by the caller.\n  sources:\n  - openapi/_original/agorapulse-open-api-openapi.yml\n- name: MCP OAuth\n  type: oauth2\n  applies_to: The remote MCP server at https://api.openmcp.agorapulse.com/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.identity.agorapulse.com/oauth/authorize\n\
  \    tokenUrl: https://api.identity.agorapulse.com/oauth/token\n    userinfoUrl: https://api.identity.agorapulse.com/oauth/userinfo\n    registrationUrl: https://api.identity.agorapulse.com/oauth/register\n    scopes: [read]\n    pkce: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    resource_parameter_supported: true\n  sources:\n  - well-known/agorapulse-oauth-authorization-server.json\n  - well-known/agorapulse-oauth-protected-resource.json\nkey_management:\n  mint: Avatar (bottom left) -> Personal settings -> API Keys -> Create new API keys\n  visibility: Shown once at creation; not retrievable afterwards.\n  scope: Per individual user; API permissions equal that user's in-app access level.\n  plan_gate: >-\n    The REST Reports Open API is documented as available on the Custom plan only. The MCP connector\n    is documented as available on every plan except Legacy and Free — a different\
  \ gate.\nx-evidence:\n- {fetched: '2026-08-13', url: 'https://api.agorapulse.com/v1.0/core/organizations', http_status: 401, body: '{\"code\":2,\"message\":\"No valid API key found in request header X-API-Key\"}'}\n- {fetched: '2026-08-13', url: 'https://api.openmcp.agorapulse.com/.well-known/oauth-authorization-server', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/authentication/agorapulse-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Social Media Management
- Social-Media
- CRM
- Analytics
- Publishing
- Inbox Management
- Social Listening
---
