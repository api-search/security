---
api_key_in: []
auth_types: []
description: Allego's API surface is authenticated with OAuth 2.0. This profile is built from documents Allego actually publishes — the RFC 8414 Authorization Server Metadata and RFC 9728 Protected Resource Metadata served by the Allego MCP API Server — plus the live HTTP behaviour of the REST surface at my.allego.com/rest/. Allego publishes no public API reference and no OpenAPI, so no securityScheme block could be derived from a spec; every field below was read off a real response.
kind: authentication
layout: security
method: probed
name: Allego Authentication
name_suffix: Authentication
oauth_flows: []
overview: Allego declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Allego
provider_slug: allego
scheme_count: 3
schemes:
- applies_to:
  - https://mcp.allego.com/mcp
  - https://my.allego.com/rest/
  authorization_endpoint: https://my.allego.com/mcp/oauth2/authorize.do
  code_challenge_methods_supported:
  - S256
  description: OAuth 2.0 / 2.1 authorization-code and client-credentials flows, PKCE S256 required, with RFC 7591 dynamic client registration. Advertised by Allego's own authorization server metadata document.
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  id: allego-oauth2
  issuer: https://mcp.allego.com
  method: probed
  registration_endpoint: https://my.allego.com/rest/oauth2/register
  response_types_supported:
  - code
  scopes: []
  scopes_note: scopes_supported is published as an empty array. Allego documents no OAuth scope vocabulary publicly, so no scopes/ artifact was derived.
  source: https://mcp.allego.com/.well-known/oauth-authorization-server
  token_endpoint: https://my.allego.com/rest/oauth2/token
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
- applies_to:
  - https://mcp.allego.com/mcp
  description: 'Bearer token in the Authorization header. Declared by Allego''s protected-resource metadata (bearer_methods_supported: ["header"]) and confirmed by the WWW-Authenticate challenge returned by the MCP endpoint.'
  id: allego-bearer
  method: probed
  scheme: bearer
  source: https://mcp.allego.com/.well-known/oauth-protected-resource
  type: http
- applies_to:
  - https://my.allego.com/rest/
  description: The REST surface at https://my.allego.com/rest/ also accepts the interactive application session. An unauthenticated request returns HTTP 401 with the Allego JSON error envelope and the message "Your session has expired. Please sign in again.", and browser access to /help/ 302s to https://my.allego.com/login.do.
  id: allego-session
  method: probed
  source: https://my.allego.com/rest/
  type: session
slug: allego-authentication
source_filename: allego-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Allego Authentication\ndescription: >-\n  Allego's API surface is authenticated with OAuth 2.0. This profile is built from\n  documents Allego actually publishes — the RFC 8414 Authorization Server Metadata and\n  RFC 9728 Protected Resource Metadata served by the Allego MCP API Server — plus the live\n  HTTP behaviour of the REST surface at my.allego.com/rest/. Allego publishes no public API\n  reference and no OpenAPI, so no securityScheme block could be derived from a spec; every\n  field below was read off a real response.\ngenerated: '2026-08-14'\nmethod: probed\nsource: https://mcp.allego.com/.well-known/oauth-authorization-server\ndocs: https://www.allego.com/platform/integrations/\nschemes:\n  - id: allego-oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 / 2.1 authorization-code and client-credentials flows, PKCE S256 required,\n      with RFC 7591 dynamic client registration. Advertised by Allego's own authorization\n      server metadata document.\n\
  \    issuer: https://mcp.allego.com\n    authorization_endpoint: https://my.allego.com/mcp/oauth2/authorize.do\n    token_endpoint: https://my.allego.com/rest/oauth2/token\n    registration_endpoint: https://my.allego.com/rest/oauth2/register\n    response_types_supported:\n      - code\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n    code_challenge_methods_supported:\n      - S256\n    token_endpoint_auth_methods_supported:\n      - none\n      - client_secret_post\n      - client_secret_basic\n    scopes: []\n    scopes_note: >-\n      scopes_supported is published as an empty array. Allego documents no OAuth scope\n      vocabulary publicly, so no scopes/ artifact was derived.\n    applies_to:\n      - https://mcp.allego.com/mcp\n      - https://my.allego.com/rest/\n    source: https://mcp.allego.com/.well-known/oauth-authorization-server\n    method: probed\n  - id: allego-bearer\n    type: http\n    scheme: bearer\n  \
  \  description: >-\n      Bearer token in the Authorization header. Declared by Allego's protected-resource\n      metadata (bearer_methods_supported: [\"header\"]) and confirmed by the\n      WWW-Authenticate challenge returned by the MCP endpoint.\n    applies_to:\n      - https://mcp.allego.com/mcp\n    source: https://mcp.allego.com/.well-known/oauth-protected-resource\n    method: probed\n  - id: allego-session\n    type: session\n    description: >-\n      The REST surface at https://my.allego.com/rest/ also accepts the interactive\n      application session. An unauthenticated request returns HTTP 401 with the Allego JSON\n      error envelope and the message \"Your session has expired. Please sign in again.\",\n      and browser access to /help/ 302s to https://my.allego.com/login.do.\n    applies_to:\n      - https://my.allego.com/rest/\n    source: https://my.allego.com/rest/\n    method: probed\nenterprise_identity:\n  single_sign_on:\n    supported: true\n    description: Enterprise\
  \ Single Sign-On is listed under Human Resources and Identity integrations.\n    source: https://www.allego.com/platform/integrations/\n  provisioning:\n    scim: true\n    bulk_import: true\n    description: >-\n      \"SCIM, bulk provisioning, and secure imports\" and \"Automated onboarding and lifecycle\n      management\" are published on the integrations page.\n    source: https://www.allego.com/platform/integrations/\n  identity_providers_named:\n    providers:\n      - Azure Active Directory\n      - Jamf Pro\n      - Microsoft Intune\n      - MobileIron\n      - ADP\n      - Kronos\n    note: Named in Allego's published integrations list; not a verified protocol claim.\n    source: https://www.allego.com/platform/integrations/\nevidence:\n  - url: https://mcp.allego.com/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-14'\n  - url: https://mcp.allego.com/.well-known/oauth-protected-resource\n    http_status: 200\n    fetched: '2026-08-14'\n  -\
  \ url: https://mcp.allego.com/mcp\n    http_status: 401\n    fetched: '2026-08-14'\n    note: WWW-Authenticate Bearer challenge with resource_metadata pointer.\n  - url: https://my.allego.com/rest/\n    http_status: 401\n    fetched: '2026-08-14'\n    note: 'application/json body: {\"status\":{\"type\":\"InvalidAccessException\",\"code\":-1,...}}'\n  - url: https://my.allego.com/.well-known/openid-configuration\n    http_status: 404\n    fetched: '2026-08-14'\n    note: No OIDC discovery document is published; the OAuth metadata is not an OIDC provider.\nnotes:\n  - >-\n    No API key scheme was found. Allego publishes no self-serve developer credentials; API\n    access is arranged through the customer's Allego instance.\n  - >-\n    The authorization and token endpoints live on my.allego.com, the customer application\n    host, while the resource server is mcp.allego.com — both Allego-controlled.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allego/refs/heads/main/authentication/allego-authentication.yml
summary_line: 3 schemes
tags:
- Sales Enablement
- Sales Training
- Video Coaching
- Content Management
- Conversation Intelligence
- Deal Intelligence
- Revenue Enablement
- Certifications
- AI
---
