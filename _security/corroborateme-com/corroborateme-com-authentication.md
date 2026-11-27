---
anonymous_access: false
api_key_in: []
api_specs:
- filename: corroborateme-com-agents-api-openapi.yml
  format: yaml
  label: CorroborateMe Agents API
  slug: corroborateme-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-agents-api-openapi.yml
- filename: corroborateme-com-billing-api-openapi.yml
  format: yaml
  label: CorroborateMe Billing API
  slug: corroborateme-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-billing-api-openapi.yml
- filename: corroborateme-com-companies-api-openapi.yml
  format: yaml
  label: CorroborateMe Companies API
  slug: corroborateme-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-companies-api-openapi.yml
- filename: corroborateme-com-console-auth-api-openapi.yml
  format: yaml
  label: CorroborateMe Console auth API
  slug: corroborateme-com-console-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-console-auth-api-openapi.yml
- filename: corroborateme-com-discovery-api-openapi.yml
  format: yaml
  label: CorroborateMe Discovery API
  slug: corroborateme-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-discovery-api-openapi.yml
- filename: corroborateme-com-integrations-api-openapi.yml
  format: yaml
  label: CorroborateMe Integrations API
  slug: corroborateme-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-integrations-api-openapi.yml
- filename: corroborateme-com-login-link-idp-api-openapi.yml
  format: yaml
  label: CorroborateMe Login-link IdP API
  slug: corroborateme-com-login-link-idp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-login-link-idp-api-openapi.yml
- filename: corroborateme-com-login-links-api-openapi.yml
  format: yaml
  label: CorroborateMe Login links API
  slug: corroborateme-com-login-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-login-links-api-openapi.yml
- filename: corroborateme-com-mcp-api-openapi.yml
  format: yaml
  label: CorroborateMe MCP API
  slug: corroborateme-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-mcp-api-openapi.yml
- filename: corroborateme-com-oidc-api-openapi.yml
  format: yaml
  label: CorroborateMe OIDC API
  slug: corroborateme-com-oidc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-oidc-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: CorroborateMe Authentication
name_suffix: Authentication
oauth_flows: []
overview: CorroborateMe secures its APIs with http, oauth2, and openIdConnect across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CorroborateMe
provider_slug: corroborateme-com
scheme_count: 7
schemes:
- description: Console session JWT, company end-user JWT, bootstrap JWT, or API key (aa_...)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/corroborateme-com-openapi.yml
  type: http
- description: 'App / agent credential sent as `Authorization: Bearer aa_...`; hashed at rest, full secret shown once on mint. Minted via POST /api/companies/{id}/keys or returned by POST /api/billing/machine-pay on the zero-human bootstrap path.'
  key_prefix: aa_
  name: Company API key
  scheme: bearer
  sources:
  - https://corroborateme.com/llms.txt
  - https://corroborateme.com/llms-full.txt
  type: http
- description: Console operator session JWT obtained after an OTP / platform login-link sign-in at https://corroborateme.com/login; manages companies, billing and keys.
  name: Console session JWT
  scheme: bearer
  sources:
  - https://corroborateme.com/llms-full.txt
  type: http
- description: Short-lived (~15m) pre-key token returned by POST /api/agents/bootstrap after the emailed 6-digit code is verified; used only to pay (POST /api/billing/machine-pay) and receive an aa_ key.
  name: Bootstrap JWT
  scheme: bearer
  sources:
  - https://corroborateme.com/llms-full.txt
  type: http
- authorizationUrl: https://corroborateme.com/api/auth/oauth2/authorize
  authorization_server_metadata: https://corroborateme.com/.well-known/oauth-authorization-server
  description: MCP hosts may use an OAuth access token with aud=https://corroborateme.com/mcp/ instead of an aa_ key. Dynamic client registration plus login-link consent; authorize with resource=https://corroborateme.com/mcp/ and a scope including mcp.
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  issuer: https://corroborateme.com/api/auth
  name: MCP OAuth
  pkce:
  - S256
  protected_resource_metadata: https://corroborateme.com/.well-known/oauth-protected-resource/mcp/
  registrationUrl: https://corroborateme.com/api/auth/oauth2/register
  sources:
  - https://corroborateme.com/llms-full.txt
  - https://corroborateme.com/.well-known/oauth-authorization-server
  tokenUrl: https://corroborateme.com/api/auth/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  type: oauth2
- description: CorroborateMe acts as an OIDC identity provider for the customer's own relying-party apps; register clients with POST /api/oidc/clients (public_client + PKCE preferred for SPAs; confidential client secrets are prefixed aas_). JWKS at /api/auth/jwks.
  name: CorroborateMe OIDC provider
  openIdConnectUrl: https://corroborateme.com/api/auth/.well-known/openid-configuration
  sources:
  - https://corroborateme.com/docs
  - https://corroborateme.com/api/auth/.well-known/openid-configuration
  type: openIdConnect
- description: Login-link end-user company session cookie / JWT (ids cu_...), separate from console users (usr_...).
  name: Company end-user session
  scheme: bearer
  sources:
  - https://corroborateme.com/llms-full.txt
  type: http
slug: corroborateme-com-authentication
source_filename: corroborateme-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corroborateme.com/llms-full.txt\ndocs: https://corroborateme.com/docs\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Console session JWT, company end-user JWT, bootstrap JWT, or API key (aa_...)\n  sources:\n  - openapi/corroborateme-com-openapi.yml\n- name: Company API key\n  type: http\n  scheme: bearer\n  key_prefix: aa_\n  description: \"App / agent credential sent as `Authorization: Bearer aa_...`; hashed at rest, full secret shown once on mint. Minted via POST /api/companies/{id}/keys or returned by POST /api/billing/machine-pay on the zero-human bootstrap path.\"\n  sources:\n  - https://corroborateme.com/llms.txt\n  - https://corroborateme.com/llms-full.txt\n- name: Console session JWT\n  type: http\n  scheme: bearer\n  description: Console operator session JWT obtained after an OTP / platform login-link sign-in at https://corroborateme.com/login;\
  \ manages companies, billing and keys.\n  sources:\n  - https://corroborateme.com/llms-full.txt\n- name: Bootstrap JWT\n  type: http\n  scheme: bearer\n  description: Short-lived (~15m) pre-key token returned by POST /api/agents/bootstrap after the emailed 6-digit code is verified; used only to pay (POST /api/billing/machine-pay) and receive an aa_ key.\n  sources:\n  - https://corroborateme.com/llms-full.txt\n- name: MCP OAuth\n  type: oauth2\n  description: MCP hosts may use an OAuth access token with aud=https://corroborateme.com/mcp/ instead of an aa_ key. Dynamic client registration plus login-link consent; authorize with resource=https://corroborateme.com/mcp/ and a scope including mcp.\n  protected_resource_metadata: https://corroborateme.com/.well-known/oauth-protected-resource/mcp/\n  authorization_server_metadata: https://corroborateme.com/.well-known/oauth-authorization-server\n  issuer: https://corroborateme.com/api/auth\n  authorizationUrl: https://corroborateme.com/api/auth/oauth2/authorize\n\
  \  tokenUrl: https://corroborateme.com/api/auth/oauth2/token\n  registrationUrl: https://corroborateme.com/api/auth/oauth2/register\n  grant_types: [authorization_code, client_credentials, refresh_token]\n  pkce: [S256]\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post, private_key_jwt]\n  sources:\n  - https://corroborateme.com/llms-full.txt\n  - https://corroborateme.com/.well-known/oauth-authorization-server\n- name: CorroborateMe OIDC provider\n  type: openIdConnect\n  openIdConnectUrl: https://corroborateme.com/api/auth/.well-known/openid-configuration\n  description: CorroborateMe acts as an OIDC identity provider for the customer's own relying-party apps; register clients with POST /api/oidc/clients (public_client + PKCE preferred for SPAs; confidential client secrets are prefixed aas_). JWKS at /api/auth/jwks.\n  sources:\n  - https://corroborateme.com/docs\n  - https://corroborateme.com/api/auth/.well-known/openid-configuration\n- name: Company end-user\
  \ session\n  type: http\n  scheme: bearer\n  description: Login-link end-user company session cookie / JWT (ids cu_...), separate from console users (usr_...).\n  sources:\n  - https://corroborateme.com/llms-full.txt\n"
source_yaml_url: https://artifacts.apis.io/corroborateme-com/authentication/corroborateme-com-authentication.yml
summary_line: http/oauth2/openIdConnect · 7 schemes
tags:
- Company
- Authentication
- Identity
- Sign In
- Passkeys
- OpenID Connect
- SSO
- AI Agents
- MCP
---
