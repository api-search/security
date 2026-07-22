---
api_key_in:
- env
auth_types:
- oauth2
- apiKey
- saml2
- scim
description: ''
kind: authentication
layout: security
method: searched
name: Natoma Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Natoma secures its APIs with oauth2, apiKey, saml2, and scim across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Natoma
provider_slug: natoma
scheme_count: 4
schemes:
- authorization_url: https://api.natoma.app/oauth/authorize
  dynamic_client_registration: true
  flow: authorizationCode
  introspection_url: https://api.natoma.app/oauth/introspect
  issuer: https://api.natoma.app/oauth
  name: PlatformOAuth2
  note: OAuth 2.1-style authorization server the Natoma MCP platform advertises via RFC 8414 metadata; public clients (token_endpoint_auth_method none) with PKCE and RFC 7591 Dynamic Client Registration. Used by remote MCP clients.
  pkce:
  - S256
  - plain
  registration_url: https://api.natoma.app/oauth/register
  revocation_url: https://api.natoma.app/oauth/revoke
  token_endpoint_auth_methods:
  - none
  token_url: https://api.natoma.app/oauth/token
  type: oauth2
- in: env
  name: ApiKey
  name_field: NATOMA_MCP_API_KEY
  note: API key used by the stdio gateway (@natomalabs/natoma-mcp-gateway) to authenticate to the platform.
  type: apiKey
- name: SAML2 SSO
  note: 'SAML 2.0 SSO for the Natoma console via Microsoft Entra ID and the Okta Integration Network (OIN). Docs: entra-sso, okta-sso.'
  type: saml2
- name: SCIM
  note: SCIM 2.0 user/role provisioning from Microsoft Entra ID and Okta (group- and attribute-based role mapping to Natoma roles).
  type: scim
slug: natoma-authentication
source_filename: natoma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.natoma.app/.well-known/oauth-authorization-server\ndocs: https://docs.natoma.ai/docs/enterprise/secure-access-to-natoma\nsummary:\n  types: [oauth2, apiKey, saml2, scim]\n  api_key_in: [env]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: PlatformOAuth2\n  type: oauth2\n  flow: authorizationCode\n  issuer: https://api.natoma.app/oauth\n  authorization_url: https://api.natoma.app/oauth/authorize\n  token_url: https://api.natoma.app/oauth/token\n  registration_url: https://api.natoma.app/oauth/register\n  revocation_url: https://api.natoma.app/oauth/revoke\n  introspection_url: https://api.natoma.app/oauth/introspect\n  pkce: [S256, plain]\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [none]\n  note: >-\n    OAuth 2.1-style authorization server the Natoma MCP platform advertises via\n    RFC 8414 metadata; public clients (token_endpoint_auth_method none) with PKCE and\n    RFC 7591 Dynamic\
  \ Client Registration. Used by remote MCP clients.\n- name: ApiKey\n  type: apiKey\n  in: env\n  name_field: NATOMA_MCP_API_KEY\n  note: API key used by the stdio gateway (@natomalabs/natoma-mcp-gateway) to authenticate to the platform.\n- name: SAML2 SSO\n  type: saml2\n  note: >-\n    SAML 2.0 SSO for the Natoma console via Microsoft Entra ID and the Okta\n    Integration Network (OIN). Docs: entra-sso, okta-sso.\n- name: SCIM\n  type: scim\n  note: >-\n    SCIM 2.0 user/role provisioning from Microsoft Entra ID and Okta (group- and\n    attribute-based role mapping to Natoma roles).\nper_connector_auth: >-\n  Each catalog connector authenticates to its downstream app independently (OAuth,\n  scoped API key, service-account key, or PAT), managed centrally by Natoma.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natoma/refs/heads/main/authentication/natoma-authentication.yml
summary_line: oauth2/apiKey/saml2/scim · 4 schemes
tags:
- Company
- Cybersecurity
- Model Context Protocol
- MCP
- AI Agents
- Identity
- Access Management
- Governance
- Security
---
