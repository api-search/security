---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Reevo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Reevo secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Reevo
provider_slug: reevo
scheme_count: 3
schemes:
- applies_to: https://api.reevo.ai/api/v1/public
  authorization_model:
    enforcement: The service validates on every request that the key carries the required permissions and rejects the call with an error naming the missing permissions.
    inheritance: A write permission automatically grants read on the same resource.
    permissions:
    - read: true
      resource: Accounts
      write: true
    - read: true
      resource: Contacts
      write: true
    - read: true
      resource: Opportunities
      write: true
    - read: true
      resource: Tasks
      write: true
    - read: false
      resource: Activities
      write: true
    - read: true
      resource: Users
      write: false
    - read: true
      resource: Mailbox
      write: false
    - read: true
      resource: Sequence Enrollment
      write: true
    - read: true
      resource: Webhooks
      write: true
    style: per-resource read/write permissions selected at key creation
  in: header
  issuance:
    prerequisite: The organization must have available quota for public requests.
    revocation: Keys are expired from the API keys table (three-dot menu -> Expire key); an expired key stops working immediately.
    rotation_policy: null
    url: https://app.reevo.ai/settings/integrations
    visibility: The key is shown exactly once at creation and cannot be retrieved again.
    where: Reevo workspace Settings -> Integrations -> API Keys -> New API key
    who: workspace admins only
  name: ApiKeyAuth
  observed:
    invalid_key_body: '{"error_response_type":"GENERIC","error":"UnauthorizedError","message":"Invalid API key","details":null}'
    invalid_key_status: 401
    missing_key_body: '{"detail":[{"type":"missing","loc":["header","x-api-key"],"msg":"Field required","input":null}]}'
    missing_key_status: 422
    probe_url: https://api.reevo.ai/api/v1/public/accounts/search
    probed: '2026-08-13'
  parameter_name: x-api-key
  source: https://help.reevo.ai/Data-management-and-migration/Integrations-With-Other-Tools
  type: apiKey
- applies_to: https://mcp.reevo.ai/mcp
  authorization_servers:
  - https://mcp.reevo.ai
  bearer_methods_supported:
  - header
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.reevo.ai/authorize
    flow: authorizationCode
    refreshUrl: https://mcp.reevo.ai/token
    scopes: scopes/reevo-scopes.yml
    tokenUrl: https://mcp.reevo.ai/token
  issuer: https://mcp.reevo.ai
  metadata_documents:
  - https://mcp.reevo.ai/.well-known/oauth-authorization-server
  - https://mcp.reevo.ai/.well-known/oauth-protected-resource
  name: ReevoMCPOAuth
  note: Consent is per-scope; Reevo's authorization page shows exactly which object/action scopes a client requested and a tool can only run if that scope was granted. Tokens act as the connected Reevo user and inherit that user's workspace permissions.
  pkce:
    code_challenge_methods:
    - S256
    required: true
  protected_resource: https://mcp.reevo.ai
  registration_endpoint: https://mcp.reevo.ai/register
  resource_documentation: https://reevo.ai
  revocation_endpoint: https://mcp.reevo.ai/token
  source: https://mcp.reevo.ai/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- applies_to: https://app.reevo.ai (end-user sign-in, not an API surface)
  authorization_endpoint: https://login.reevo.ai/authorize
  code_challenge_methods:
  - S256
  - plain
  device_authorization_endpoint: https://login.reevo.ai/oauth/device/code
  issuer: https://login.reevo.ai/
  jwks_uri: https://login.reevo.ai/.well-known/jwks.json
  mfa_challenge_endpoint: https://login.reevo.ai/mfa/challenge
  name: ReevoLogin
  note: Standard OIDC discovery for Reevo's identity host. It authenticates humans into the Reevo web app; it is not the authorization server for either the public REST API (x-api-key) or the MCP server (which runs its own issuer at mcp.reevo.ai). Third-party sign-in with Microsoft is documented as an option.
  openIdConnectUrl: https://login.reevo.ai/.well-known/openid-configuration
  registration_endpoint: https://login.reevo.ai/oidc/register
  revocation_endpoint: https://login.reevo.ai/oauth/revoke
  scopes_supported:
  - openid
  - profile
  - offline_access
  - name
  - given_name
  - family_name
  - nickname
  - email
  - email_verified
  - picture
  - created_at
  - identities
  - phone
  - address
  source: https://login.reevo.ai/.well-known/openid-configuration
  token_endpoint: https://login.reevo.ai/oauth/token
  type: openIdConnect
  userinfo_endpoint: https://login.reevo.ai/userinfo
slug: reevo-authentication
source_filename: reevo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.reevo.ai/Data-management-and-migration/Integrations-With-Other-Tools\ndocs:\n- https://help.reevo.ai/Data-management-and-migration/Integrations-With-Other-Tools\n- https://help.reevo.ai/AI-and-productivity/Reevo-MCP\nnote: Reevo publishes no OpenAPI, so this profile is transcribed from the provider's\n  own documentation and confirmed against live unauthenticated probes of api.reevo.ai\n  and mcp.reevo.ai. `derive-authentication.py` was run first and produced nothing (0\n  spec files in openapi/).\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  applies_to: https://api.reevo.ai/api/v1/public\n  source: https://help.reevo.ai/Data-management-and-migration/Integrations-With-Other-Tools\n  issuance:\n    where: Reevo workspace Settings -> Integrations\
  \ -> API Keys -> New API key\n    url: https://app.reevo.ai/settings/integrations\n    who: workspace admins only\n    prerequisite: The organization must have available quota for public requests.\n    visibility: The key is shown exactly once at creation and cannot be retrieved again.\n    revocation: Keys are expired from the API keys table (three-dot menu -> Expire\n      key); an expired key stops working immediately.\n    rotation_policy: null\n  authorization_model:\n    style: per-resource read/write permissions selected at key creation\n    inheritance: A write permission automatically grants read on the same resource.\n    enforcement: The service validates on every request that the key carries the required\n      permissions and rejects the call with an error naming the missing permissions.\n    permissions:\n    - resource: Accounts\n      read: true\n      write: true\n    - resource: Contacts\n      read: true\n      write: true\n    - resource: Opportunities\n      read:\
  \ true\n      write: true\n    - resource: Tasks\n      read: true\n      write: true\n    - resource: Activities\n      read: false\n      write: true\n    - resource: Users\n      read: true\n      write: false\n    - resource: Mailbox\n      read: true\n      write: false\n    - resource: Sequence Enrollment\n      read: true\n      write: true\n    - resource: Webhooks\n      read: true\n      write: true\n  observed:\n    missing_key_status: 422\n    missing_key_body: '{\"detail\":[{\"type\":\"missing\",\"loc\":[\"header\",\"x-api-key\"],\"msg\":\"Field\n      required\",\"input\":null}]}'\n    invalid_key_status: 401\n    invalid_key_body: '{\"error_response_type\":\"GENERIC\",\"error\":\"UnauthorizedError\",\"message\":\"Invalid\n      API key\",\"details\":null}'\n    probed: '2026-08-13'\n    probe_url: https://api.reevo.ai/api/v1/public/accounts/search\n- name: ReevoMCPOAuth\n  type: oauth2\n  applies_to: https://mcp.reevo.ai/mcp\n  source: https://mcp.reevo.ai/.well-known/oauth-authorization-server\n\
  \  metadata_documents:\n  - https://mcp.reevo.ai/.well-known/oauth-authorization-server\n  - https://mcp.reevo.ai/.well-known/oauth-protected-resource\n  issuer: https://mcp.reevo.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.reevo.ai/authorize\n    tokenUrl: https://mcp.reevo.ai/token\n    refreshUrl: https://mcp.reevo.ai/token\n    scopes: scopes/reevo-scopes.yml\n  registration_endpoint: https://mcp.reevo.ai/register\n  revocation_endpoint: https://mcp.reevo.ai/token\n  dynamic_client_registration: true\n  pkce:\n    required: true\n    code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  bearer_methods_supported:\n  - header\n  protected_resource: https://mcp.reevo.ai\n  authorization_servers:\n  - https://mcp.reevo.ai\n  resource_documentation: https://reevo.ai\n  note: Consent is per-scope; Reevo's authorization page shows exactly which object/action\n    scopes a client requested\
  \ and a tool can only run if that scope was granted. Tokens\n    act as the connected Reevo user and inherit that user's workspace permissions.\n- name: ReevoLogin\n  type: openIdConnect\n  applies_to: https://app.reevo.ai (end-user sign-in, not an API surface)\n  openIdConnectUrl: https://login.reevo.ai/.well-known/openid-configuration\n  source: https://login.reevo.ai/.well-known/openid-configuration\n  issuer: https://login.reevo.ai/\n  authorization_endpoint: https://login.reevo.ai/authorize\n  token_endpoint: https://login.reevo.ai/oauth/token\n  userinfo_endpoint: https://login.reevo.ai/userinfo\n  jwks_uri: https://login.reevo.ai/.well-known/jwks.json\n  device_authorization_endpoint: https://login.reevo.ai/oauth/device/code\n  revocation_endpoint: https://login.reevo.ai/oauth/revoke\n  registration_endpoint: https://login.reevo.ai/oidc/register\n  mfa_challenge_endpoint: https://login.reevo.ai/mfa/challenge\n  code_challenge_methods:\n  - S256\n  - plain\n  scopes_supported:\n\
  \  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\n  note: Standard OIDC discovery for Reevo's identity host. It authenticates humans\n    into the Reevo web app; it is not the authorization server for either the public\n    REST API (x-api-key) or the MCP server (which runs its own issuer at mcp.reevo.ai).\n    Third-party sign-in with Microsoft is documented as an option.\ngaps:\n- No OpenAPI securitySchemes block exists, so no machine-readable auth contract is\n  published for the REST API.\n- No documented API key rotation policy, key expiry period, or IP allow-listing.\n- No mTLS, HTTP basic or bearer-JWT option is documented for the REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reevo/refs/heads/main/authentication/reevo-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Artificial Intelligence
- Sales
- CRM
- Revenue Operations
- Sales Automation
- Lead Generation
- Agents
- MCP
- Sales Engagement
---
