---
api_key_in:
- header
api_specs:
- filename: spekit-openapi.yml
  format: yaml
  label: Spekit API
  slug: spekit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Spekit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spekit secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spekit
provider_slug: spekit
scheme_count: 2
schemes:
- description: Token-based authentication with required prefix "Token"
  example_header: 'Authorization: Token <your-api-token>'
  in: header
  issuance:
    auditable: Token generation and revocation are themselves activity types on the API — filter v1_analytics_user_activities_list by api_auth_token_generated / api_auth_token_revoked.
    revocable: true
    steps:
    - Enter a description for the token (e.g. "Tableau Reporting Sync").
    - Set a custom expiration period, from 1 week through "Never Expire".
    - Click Generate new token.
    - Copy the token immediately — it is shown once and cannot be retrieved later.
    where: Spekit Web App, Settings then API Tokens
    who: Spekit Account Admins only
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/spekit-openapi.yml
  surface: REST API (https://api.spekit.co)
  type: apiKey
- access_token_lifetime: 24 hours
  authorization_model: Delegated only. The connector grants no new access — every call runs as the signed-in user within that user's existing Spekit role, enforced at the backend API layer. Scope cannot be narrowed to specific topics or deal rooms, and there is no forced read-only mode independent of role.
  bearer_methods_supported:
  - header
  client_credentials: false
  client_credentials_note: Spekit states explicitly there is no machine-to-machine path using a Client ID and secret — every connection requires an interactive sign-in and consent with the user's own Spekit login.
  client_id_metadata_document_supported: true
  discovery:
  - file: ../well-known/spekit-mcp-oauth-authorization-server.json
    path: /.well-known/oauth-authorization-server
    rfc: RFC 8414
  - advertised_via: WWW-Authenticate resource_metadata on the 401
    file: ../well-known/spekit-mcp-oauth-protected-resource.json
    path: /.well-known/oauth-protected-resource/mcp
    rfc: RFC 9728
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.spekit.co/authorize
    flow: authorizationCode
    pkce: required (S256)
    scopes:
    - openid
    - profile
    - email
    - read
    tokenUrl: https://mcp.spekit.co/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.spekit.co/
  name: mcp-oauth2
  refresh_token_lifetime: 30 days, rotating on every use; each refresh cancels the prior token
  registration_endpoint: https://mcp.spekit.co/register
  revocation: users or org admins can disconnect at any time, like any other OAuth grant
  session_state: encrypted at rest (Fernet) in the session store
  sources:
  - https://mcp.spekit.co/.well-known/oauth-authorization-server
  - https://help.spekit.com/hc/en-us/articles/53991678945435-Spekit-MCP-Data-Privacy-Security-FAQs
  surface: MCP connector (https://mcp.spekit.co/mcp)
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  token_format: RS256-signed JWT, verified against the identity provider's published JWKS with issuer and audience claim checks
  type: oauth2
slug: spekit-authentication
source_filename: spekit-authentication.yml
source_heading: Authentication Profile
source_url: https://api.spekit.co/api-schema/
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/spekit-openapi.yml\ndocs: https://help.spekit.com/hc/en-us/articles/31041891807643-Spekit-API-Overview\nsources:\n- https://api.spekit.co/api-schema/\n- https://help.spekit.com/hc/en-us/articles/31041891807643-Spekit-API-Overview\n- https://help.spekit.com/hc/en-us/articles/53991678945435-Spekit-MCP-Data-Privacy-Security-FAQs\n- https://mcp.spekit.co/.well-known/oauth-authorization-server\n- https://mcp.spekit.co/.well-known/oauth-protected-resource/mcp\nnote: >-\n  Spekit runs two independent auth models on two independent surfaces. The REST API\n  (api.spekit.co) uses a long-lived admin-issued static token. The MCP connector\n  (mcp.spekit.co) uses OAuth 2.0 authorization code with PKCE and dynamic client registration,\n  with no machine-to-machine path at all. A credential for one does not work on the other.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n\
  schemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  surface: REST API (https://api.spekit.co)\n  description: Token-based authentication with required prefix \"Token\"\n  example_header: 'Authorization: Token <your-api-token>'\n  issuance:\n    who: Spekit Account Admins only\n    where: Spekit Web App, Settings then API Tokens\n    steps:\n    - Enter a description for the token (e.g. \"Tableau Reporting Sync\").\n    - Set a custom expiration period, from 1 week through \"Never Expire\".\n    - Click Generate new token.\n    - Copy the token immediately — it is shown once and cannot be retrieved later.\n    revocable: true\n    auditable: >-\n      Token generation and revocation are themselves activity types on the API — filter\n      v1_analytics_user_activities_list by api_auth_token_generated / api_auth_token_revoked.\n  sources:\n  - openapi/spekit-openapi.yml\n- name: mcp-oauth2\n  type: oauth2\n  surface: MCP connector (https://mcp.spekit.co/mcp)\n\
  \  issuer: https://mcp.spekit.co/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.spekit.co/authorize\n    tokenUrl: https://mcp.spekit.co/token\n    pkce: required (S256)\n    scopes: [openid, profile, email, read]\n  registration_endpoint: https://mcp.spekit.co/register\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  grant_types_supported: [authorization_code, refresh_token]\n  bearer_methods_supported: [header]\n  client_credentials: false\n  client_credentials_note: >-\n    Spekit states explicitly there is no machine-to-machine path using a Client ID and secret —\n    every connection requires an interactive sign-in and consent with the user's own Spekit login.\n  access_token_lifetime: 24 hours\n  refresh_token_lifetime: 30 days, rotating on every use; each refresh cancels the prior token\n  token_format: RS256-signed JWT, verified against\
  \ the identity provider's published JWKS with issuer and audience claim checks\n  session_state: encrypted at rest (Fernet) in the session store\n  revocation: users or org admins can disconnect at any time, like any other OAuth grant\n  authorization_model: >-\n    Delegated only. The connector grants no new access — every call runs as the signed-in user\n    within that user's existing Spekit role, enforced at the backend API layer. Scope cannot be\n    narrowed to specific topics or deal rooms, and there is no forced read-only mode independent\n    of role.\n  discovery:\n  - path: /.well-known/oauth-authorization-server\n    rfc: RFC 8414\n    file: ../well-known/spekit-mcp-oauth-authorization-server.json\n  - path: /.well-known/oauth-protected-resource/mcp\n    rfc: RFC 9728\n    file: ../well-known/spekit-mcp-oauth-protected-resource.json\n    advertised_via: WWW-Authenticate resource_metadata on the 401\n  sources:\n  - https://mcp.spekit.co/.well-known/oauth-authorization-server\n\
  \  - https://help.spekit.com/hc/en-us/articles/53991678945435-Spekit-MCP-Data-Privacy-Security-FAQs\nsso:\n  note: >-\n    End-user authentication into the Spekit web app supports SAML SSO and SCIM provisioning\n    with Okta, Entra ID (Azure) and OneLogin. This is workforce identity, not API credentialing —\n    neither surface above accepts an SSO assertion directly.\n  docs: https://help.spekit.com/hc/en-us/articles/9923374365723-SSO-Overview-Configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/authentication/spekit-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Software-as-a-Service
- Sales Enablement
- Revenue Enablement
- Digital Adoption
- Knowledge-Management
- MCP
- Artificial Intelligence
- Analytics
- Sales
- Content Management
- Agents
- Authentication
---
