---
api_key_in:
- header
- query
api_specs:
- filename: workfront-planning-v2-openapi.json
  format: json
  label: Adobe Workfront Planning API v2
  slug: workfront-planning-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/openapi/workfront-planning-v2-openapi.json
- filename: workfront-planning-v1-openapi.json
  format: json
  label: Adobe Workfront Planning API v1
  slug: workfront-planning-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/openapi/workfront-planning-v1-openapi.json
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Workfront Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- jwtBearer
overview: Adobe Workfront secures its APIs with http, apiKey, and oauth2 across 8 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and jwtBearer flow(s).
provider_name: Adobe Workfront
provider_slug: workfront
scheme_count: 8
schemes:
- api: Adobe Workfront API (/attask/api)
  description: The documented preferred method for the core API. A session token is passed in a SessionID request header. Adobe calls this out as CSRF-safe and cache-friendly, unlike the URI form.
  in: header
  name: SessionID header
  parameter_name: SessionID
  status: current
  type: apiKey
- api: Adobe Workfront API (/attask/api)
  description: The same cookie the Workfront web UI uses. Adobe restricts this to read-only operations as a CSRF mitigation.
  name: Cookie-based session
  restrictions: read-only operations only
  scheme: cookie
  status: current
  type: http
- api: Adobe Workfront API (/attask/api)
  description: Legacy authentication. Adobe explicitly states it "no longer recommends the use of the /login endpoint or API keys" and directs integrators to JWT server auth or OAuth2 user auth instead. Not supported at all by the Workfront Planning API.
  in: query
  name: /login endpoint + API key
  parameter_name: apiKey
  status: deprecated
  type: apiKey
- api: Adobe Workfront API, Workfront Planning API
  description: For integrations acting on behalf of a specific user. Requires an OAuth2 application registered in Workfront (Setup > Systems > OAuth2 Applications) or an OAuth Web App / Single Page App credential in the Adobe Developer Console. PKCE variant documented separately.
  docs: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-notes/oauth-app-code-token-flow
  flow: authorizationCode
  name: OAuth2 authorization code (user authentication)
  status: current
  type: oauth2
- api: Adobe Workfront API
  docs: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-notes/oauth-app-pkce-flow
  flow: authorizationCode
  name: OAuth2 authorization code with PKCE
  pkce: true
  status: current
  type: oauth2
- api: Adobe Workfront API, Workfront Planning API
  description: For automated integrations and backend services with no user interaction. A public/ private key pair is generated, a JWT signed with the private key is exchanged for an access token. Credentials are created in the Adobe Developer Console.
  docs: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-notes/oauth-app-jwt-flow
  flow: clientCredentials
  name: OAuth2 server-to-server (JWT / client credentials)
  status: current
  type: oauth2
- api: Adobe Workfront Event Subscription API
  description: Creating, querying or deleting an event subscription requires a sessionID header AND a System Administrator access level. Outbound event messages carry a customer-supplied authToken.
  in: header
  name: Event Subscription API session
  parameter_name: sessionID
  status: current
  type: apiKey
- api: Adobe Workfront MCP Server
  authorization_endpoint: https://mcp.workfront.adobe.com/oauth/authorize
  bearer_methods_supported:
  - header
  description: The MCP endpoint returns a 401 with an RFC 9728 WWW-Authenticate challenge to unauthenticated callers, pointing at its protected-resource metadata. Dynamic client registration is open.
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  jwks_uri: https://mcp.workfront.adobe.com/oauth/jwks
  name: MCP OAuth 2.1 bearer
  pkce:
  - S256
  registration_endpoint: https://mcp.workfront.adobe.com/mcp/v1/oauth/register
  resource_indicators_supported: true
  revocation_endpoint: https://ims-na1.adobelogin.com/ims/revoke
  sources:
  - well-known/workfront-oauth-authorization-server.json
  - well-known/workfront-oauth-protected-resource.json
  status: current
  token_endpoint: https://mcp.workfront.adobe.com/oauth/token
  type: oauth2
slug: workfront-authentication
source_filename: workfront-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-general-information/api-basics\ndocs:\n- https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-general-information/api-basics\n- https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/configure-integrations/create-oauth-application\n- https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-notes/oauth-app-code-token-flow\n- https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-general-information/planning-api-basics\nnote: Neither published Workfront Planning OpenAPI declares a components.securitySchemes block, so\n  nothing could be derived mechanically (derive-authentication.py returned zero schemes). This profile\n  is read from the Workfront and Adobe Developer Console documentation and from the live\
  \ OAuth\n  discovery documents served by the MCP host, which are the only machine-readable auth metadata\n  Workfront publishes.\nsummary:\n  types: [http, apiKey, oauth2]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode, clientCredentials, jwtBearer]\n  identity_provider: Adobe IMS (ims-na1.adobelogin.com)\n  deprecated: [apiKey, sessionID-via-login-endpoint]\nschemes:\n- name: SessionID header\n  api: Adobe Workfront API (/attask/api)\n  type: apiKey\n  in: header\n  parameter_name: SessionID\n  description: The documented preferred method for the core API. A session token is passed in a\n    SessionID request header. Adobe calls this out as CSRF-safe and cache-friendly, unlike the URI\n    form.\n  status: current\n- name: Cookie-based session\n  api: Adobe Workfront API (/attask/api)\n  type: http\n  scheme: cookie\n  description: The same cookie the Workfront web UI uses. Adobe restricts this to read-only\n    operations as a CSRF mitigation.\n  status: current\n\
  \  restrictions: read-only operations only\n- name: /login endpoint + API key\n  api: Adobe Workfront API (/attask/api)\n  type: apiKey\n  in: query\n  parameter_name: apiKey\n  description: Legacy authentication. Adobe explicitly states it \"no longer recommends the use of the\n    /login endpoint or API keys\" and directs integrators to JWT server auth or OAuth2 user auth\n    instead. Not supported at all by the Workfront Planning API.\n  status: deprecated\n- name: OAuth2 authorization code (user authentication)\n  api: Adobe Workfront API, Workfront Planning API\n  type: oauth2\n  flow: authorizationCode\n  description: For integrations acting on behalf of a specific user. Requires an OAuth2 application\n    registered in Workfront (Setup > Systems > OAuth2 Applications) or an OAuth Web App / Single Page\n    App credential in the Adobe Developer Console. PKCE variant documented separately.\n  docs: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-notes/oauth-app-code-token-flow\n\
  \  status: current\n- name: OAuth2 authorization code with PKCE\n  api: Adobe Workfront API\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  docs: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-notes/oauth-app-pkce-flow\n  status: current\n- name: OAuth2 server-to-server (JWT / client credentials)\n  api: Adobe Workfront API, Workfront Planning API\n  type: oauth2\n  flow: clientCredentials\n  description: For automated integrations and backend services with no user interaction. A public/\n    private key pair is generated, a JWT signed with the private key is exchanged for an access token.\n    Credentials are created in the Adobe Developer Console.\n  docs: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-api/api-notes/oauth-app-jwt-flow\n  status: current\n- name: Event Subscription API session\n  api: Adobe Workfront Event Subscription API\n  type: apiKey\n  in: header\n  parameter_name: sessionID\n  description:\
  \ Creating, querying or deleting an event subscription requires a sessionID header AND a\n    System Administrator access level. Outbound event messages carry a customer-supplied authToken.\n  status: current\n- name: MCP OAuth 2.1 bearer\n  api: Adobe Workfront MCP Server\n  type: oauth2\n  flow: authorizationCode\n  pkce: [S256]\n  bearer_methods_supported: [header]\n  authorization_endpoint: https://mcp.workfront.adobe.com/oauth/authorize\n  token_endpoint: https://mcp.workfront.adobe.com/oauth/token\n  jwks_uri: https://mcp.workfront.adobe.com/oauth/jwks\n  registration_endpoint: https://mcp.workfront.adobe.com/mcp/v1/oauth/register\n  revocation_endpoint: https://ims-na1.adobelogin.com/ims/revoke\n  grant_types_supported: [authorization_code, refresh_token]\n  resource_indicators_supported: true\n  description: The MCP endpoint returns a 401 with an RFC 9728 WWW-Authenticate challenge to\n    unauthenticated callers, pointing at its protected-resource metadata. Dynamic client registration\n\
  \    is open.\n  sources:\n  - well-known/workfront-oauth-authorization-server.json\n  - well-known/workfront-oauth-protected-resource.json\n  status: current\nscopes: scopes/workfront-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/authentication/workfront-authentication.yml
summary_line: http/apiKey/oauth2 · 8 schemes
tags:
- Company
- Work Management
- Project Management
- Marketing Operations
- Creative Operations
- Collaboration
- Approvals
- Resource Management
- Workflow-Automation
- Enterprise Software
- Adobe
- MCP
---
