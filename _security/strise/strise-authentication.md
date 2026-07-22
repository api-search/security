---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Strise Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Strise secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Strise
provider_slug: strise
scheme_count: 3
schemes:
- description: The Connect API (https://graphql.strise.ai/connect/graphql) authenticates requests with a bearer access token in the Authorization header. Access is provisioned by Strise; request via tech@strise.ai.
  docs: https://docs.strise.ai/technology/strise-connect-api/
  name: ConnectApiBearer
  scheme: bearer
  surface: Strise Connect API (GraphQL)
  type: http
- description: 'The MCP server is an OAuth 2.0 protected resource. Clients register dynamically (RFC 7591), authorize with PKCE (S256) against Auth0 using the same credentials as the Strise web app, and present Authorization: Bearer <token>. Optional X-Strise-Team header selects the acting team.'
  docs: https://docs.strise.ai/mcp/
  flows:
  - authorizationUrl: https://mcp.strise.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://mcp.strise.ai/oauth/register
    scopes:
      email: Email address
      offline_access: Refresh-token issuance
      openid: OpenID Connect authentication
      profile: Basic profile information
    tokenUrl: https://mcp.strise.ai/oauth/token
  name: McpOAuth
  provider: Auth0
  surface: Strise MCP server (https://mcp.strise.ai/mcp)
  type: oauth2
- description: Web login supports SSO via Auth0 with OIDC. Email-domain redirection routes users to their IdP (e.g. Microsoft Entra ID); Microsoft and Google OIDC buttons are also offered.
  docs: https://docs.strise.ai/technology/single-sign-on/
  name: SingleSignOn
  provider: Auth0
  surface: Strise web application (app.strise.ai)
  type: openIdConnect
slug: strise-authentication
source_filename: strise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.strise.ai/technology/strise-connect-api/, https://docs.strise.ai/mcp/, https://docs.strise.ai/technology/single-sign-on/\nsummary:\n  types: [http, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Strise has no OpenAPI (the Connect API is GraphQL), so this profile is\n    captured from the documentation rather than derived from a spec.\nschemes:\n- name: ConnectApiBearer\n  surface: Strise Connect API (GraphQL)\n  type: http\n  scheme: bearer\n  description: >-\n    The Connect API (https://graphql.strise.ai/connect/graphql) authenticates\n    requests with a bearer access token in the Authorization header. Access is\n    provisioned by Strise; request via tech@strise.ai.\n  docs: https://docs.strise.ai/technology/strise-connect-api/\n- name: McpOAuth\n  surface: Strise MCP server (https://mcp.strise.ai/mcp)\n  type: oauth2\n  provider: Auth0\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://mcp.strise.ai/oauth/authorize\n    tokenUrl: https://mcp.strise.ai/oauth/token\n    registrationUrl: https://mcp.strise.ai/oauth/register   # RFC 7591 dynamic client registration\n    pkce: S256\n    scopes:\n      openid: OpenID Connect authentication\n      profile: Basic profile information\n      email: Email address\n      offline_access: Refresh-token issuance\n  description: >-\n    The MCP server is an OAuth 2.0 protected resource. Clients register\n    dynamically (RFC 7591), authorize with PKCE (S256) against Auth0 using the\n    same credentials as the Strise web app, and present Authorization: Bearer\n    <token>. Optional X-Strise-Team header selects the acting team.\n  docs: https://docs.strise.ai/mcp/\n- name: SingleSignOn\n  surface: Strise web application (app.strise.ai)\n  type: openIdConnect\n  provider: Auth0\n  description: >-\n    Web login supports SSO via Auth0 with OIDC. Email-domain redirection routes\n    users to their IdP (e.g.\
  \ Microsoft Entra ID); Microsoft and Google OIDC\n    buttons are also offered.\n  docs: https://docs.strise.ai/technology/single-sign-on/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strise/refs/heads/main/authentication/strise-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Fintech
- RegTech
- AML
- KYC
- KYB
- Compliance
- Financial Crime
- Screening
- Sanctions
- PEP
- GraphQL
- MCP
---
