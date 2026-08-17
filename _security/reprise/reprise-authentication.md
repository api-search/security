---
api_key_in:
- query
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Reprise Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Reprise secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Reprise
provider_slug: reprise
scheme_count: 2
schemes:
- api: reprise:mcp
  bearer_methods_supported:
  - header
  code_challenge_methods_supported:
  - S256
  consent: explicit per-user consent screen
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://app.getreprise.com/r/mcp/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://app.getreprise.com/r/mcp/oauth/register
    tokenUrl: https://app.getreprise.com/r/mcp/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  identity: 'Tokens are scoped to the authorizing user and inherit that user''s existing Reprise role. The MCP cannot perform any action the user could not already perform in the Reprise UI. No new license is required; a Builder license builds, a Presenter license presents.

    '
  issuer: https://app.getreprise.com
  name: MCPOAuth2
  pkce: required
  resource: https://app.getreprise.com/mcp
  response_types_supported:
  - code
  revocation: 'IdP-driven deprovisioning revokes tokens immediately. SCIM/IdP deactivation cascades to access and refresh tokens, and the token-verify filter checks user.is_active on every request, so there is no expiry-only window. The connection is also listed in the user''s authorized-apps view and revocable there.

    '
  sources:
  - well-known/reprise-oauth-authorization-server.json
  - well-known/reprise-oauth-protected-resource.json
  - https://reprise.zendesk.com/hc/en-us/articles/50081170817691-The-Reprise-MCP-Meet-your-AI-Demo-Engineer
  storage: No tokens or credentials are stored in the AI client or shared with third parties
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- api:
  - reprise:data-api
  - reprise:html-environment-data-api
  description: 'Both analytics Data APIs authenticate with an opaque token appended to the endpoint URL as a token query parameter. For the HTML Environment Data API the customer creates the token themselves in the Reprise portal under Settings → API Management, then copies the complete endpoint (including portal ID and token) from the demo''s three-dot menu via Copy API Endpoint. For the Clone Environment Data API the token is issued by the customer''s Reprise CSM rather than self-service.

    '
  in: query
  name: DataApiToken
  name_param: token
  provisioning:
  - self-service: Settings → API Management → create new token (HTML Environment)
  - assisted: request from your Reprise CSM (Clone Environment)
  rotation: not documented
  scope: per Reprise portal / client
  sources:
  - https://reprise.zendesk.com/hc/en-us/articles/18940321925659-HTML-Environment-Data-API
  - https://reprise.zendesk.com/hc/en-us/articles/28931374746907-Clone-Environment-Data-API
  transport: HTTPS only
  type: apiKey
slug: reprise-authentication
source_filename: reprise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://reprise.zendesk.com/hc/en-us/articles/50081170817691-The-Reprise-MCP-Meet-your-AI-Demo-Engineer\ndocs:\n  - https://reprise.zendesk.com/hc/en-us/articles/50081170817691-The-Reprise-MCP-Meet-your-AI-Demo-Engineer\n  - https://reprise.zendesk.com/hc/en-us/articles/18940321925659-HTML-Environment-Data-API\n  - https://reprise.zendesk.com/hc/en-us/articles/28931374746907-Clone-Environment-Data-API\n  - https://reprise.zendesk.com/hc/en-us/articles/26132466512155-SAML-SSO\nnote: >\n  Reprise publishes no OpenAPI, so this profile is searched from the provider's own help centre\n  and from two live /.well-known/ documents on app.getreprise.com rather than derived from\n  securitySchemes. Reprise runs two distinct auth models: OAuth 2.0 authorization code with PKCE\n  for the MCP server, and opaque per-portal tokens on a query string for the two analytics\n  Data APIs.\n\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [query]\n\
  \  oauth2_flows: [authorizationCode]\n  human_sso: [SAML 2.0, Okta]\n\nschemes:\n  - name: MCPOAuth2\n    type: oauth2\n    api: reprise:mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.getreprise.com/r/mcp/oauth/authorize\n        tokenUrl: https://app.getreprise.com/r/mcp/oauth/token\n        registrationUrl: https://app.getreprise.com/r/mcp/oauth/register\n    issuer: https://app.getreprise.com\n    resource: https://app.getreprise.com/mcp\n    pkce: required\n    code_challenge_methods_supported: [S256]\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    token_endpoint_auth_methods_supported: [none]\n    dynamic_client_registration: true\n    bearer_methods_supported: [header]\n    consent: explicit per-user consent screen\n    identity: >\n      Tokens are scoped to the authorizing user and inherit that user's existing Reprise role.\n      The MCP cannot perform any action the user could\
  \ not already perform in the Reprise UI.\n      No new license is required; a Builder license builds, a Presenter license presents.\n    revocation: >\n      IdP-driven deprovisioning revokes tokens immediately. SCIM/IdP deactivation cascades to\n      access and refresh tokens, and the token-verify filter checks user.is_active on every\n      request, so there is no expiry-only window. The connection is also listed in the user's\n      authorized-apps view and revocable there.\n    storage: No tokens or credentials are stored in the AI client or shared with third parties\n    sources:\n      - well-known/reprise-oauth-authorization-server.json\n      - well-known/reprise-oauth-protected-resource.json\n      - https://reprise.zendesk.com/hc/en-us/articles/50081170817691-The-Reprise-MCP-Meet-your-AI-Demo-Engineer\n\n  - name: DataApiToken\n    type: apiKey\n    in: query\n    name_param: token\n    api: [reprise:data-api, reprise:html-environment-data-api]\n    description: >\n      Both\
  \ analytics Data APIs authenticate with an opaque token appended to the endpoint URL as\n      a token query parameter. For the HTML Environment Data API the customer creates the token\n      themselves in the Reprise portal under Settings → API Management, then copies the complete\n      endpoint (including portal ID and token) from the demo's three-dot menu via Copy API\n      Endpoint. For the Clone Environment Data API the token is issued by the customer's Reprise\n      CSM rather than self-service.\n    provisioning:\n      - self-service: Settings → API Management → create new token (HTML Environment)\n      - assisted: request from your Reprise CSM (Clone Environment)\n    scope: per Reprise portal / client\n    rotation: not documented\n    transport: HTTPS only\n    sources:\n      - https://reprise.zendesk.com/hc/en-us/articles/18940321925659-HTML-Environment-Data-API\n      - https://reprise.zendesk.com/hc/en-us/articles/28931374746907-Clone-Environment-Data-API\n\nhuman_authentication:\n\
  \  - name: SAML 2.0 SSO\n    type: saml2\n    binding: service-provider-initiated\n    login_url: https://app.getreprise.com/auth/login/\n    entity_id: https://app.getreprise.com/\n    acs_url: https://app.getreprise.com/auth/complete/saml/\n    required_attributes: [email, first_name, last_name]\n    enablement: requested through support@reprise.com; Reprise returns a RelayState value and its X.509 certificate\n    source: https://reprise.zendesk.com/hc/en-us/articles/26132466512155-SAML-SSO\n  - name: Okta connector\n    type: oidc-or-saml\n    note: Reprise lists a dedicated Okta connector in its integrations overview\n    source: https://reprise.zendesk.com/hc/en-us/articles/8665755587227-Integrations-Overview\n\nauthorization:\n  model: RBAC\n  note: >\n    Reprise ships role-based access control in every package with customizable roles, plus\n    builder/presenter license tiers, group sharing and folder-level permissions. MCP tokens\n    inherit whatever the authorizing user already\
  \ has.\n  sources:\n    - https://www.reprise.com/platform/enterprise-scale-and-security\n    - https://reprise.zendesk.com/hc/en-us/articles/8698959505563-Understand-Default-Roles\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n    - url: https://app.getreprise.com/.well-known/oauth-authorization-server\n      http_status: 200\n    - url: https://app.getreprise.com/.well-known/oauth-protected-resource\n      http_status: 200\n    - url: https://app.getreprise.com/mcp/\n      http_status: 401\n      note: WWW-Authenticate Bearer with RFC 9728 resource_metadata challenge\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reprise/refs/heads/main/authentication/reprise-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Demo Automation
- Product Tours
- Sales Demos
- Interactive Demos
- Sandbox Environments
- Enterprise Sales
- Marketing Technology
- Sales Enablement
- Model Context Protocol
- Agent Tooling
- Demo Analytics
---
