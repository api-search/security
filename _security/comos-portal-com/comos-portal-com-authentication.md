---
anonymous_access: true
api_key_in: []
api_specs:
- filename: comos-portal-com-openapi.yml
  format: yaml
  label: ComOS Federation Gateway
  slug: comos-federation-gateway
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comos-portal-com/openapi/comos-portal-com-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ComOS Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComOS declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ComOS
provider_slug: comos-portal-com
scheme_count: 3
schemes:
- description: Discovery, shopping, and read-only introspection need no token.
  name: anonymous
  type: none
- authorizationUrl: https://comos-portal.com/oauth/authorize
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  issuer: https://mcp.comos-federation.com
  metadata: https://comos-portal.com/.well-known/oauth-authorization-server
  name: ComOS OAuth 2.1
  pkce:
  - S256
  protected_resource_metadata: https://comos-portal.com/.well-known/oauth-protected-resource
  scopes_ref: scopes/comos-portal-com-scopes.yml
  tokenUrl: https://comos-portal.com/oauth/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  type: oauth2
- description: 'Self-hosted node calls (e.g. federation_node_report_in) are NODE-SIGNED rather than operator-token''d: the node signs the canonical envelope { node_id, nonce, timestamp, route } (OpenAPI description).'
  name: node signature
  type: signature
slug: comos-portal-com-authentication
source_filename: comos-portal-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://comos-portal.com/.well-known/oauth-authorization-server\n- https://comos-portal.com/.well-known/oauth-protected-resource\n- https://comos-portal.com/.well-known/mcp/server-card.json\n- https://comos-portal.com/security\n- https://comos-portal.com/ai.txt\ndocs: https://comos-portal.com/security\nsummary: Discovery, shopping and read-only introspection tools need no token; privileged writes use OAuth 2.1 + PKCE with per-tool scopes, and tokenless writes deny (llms.txt / ai.txt). The OpenAPI itself declares no securitySchemes.\nschemes:\n- type: none\n  name: anonymous\n  description: Discovery, shopping, and read-only introspection need no token.\n- type: oauth2\n  name: ComOS OAuth 2.1\n  issuer: https://mcp.comos-federation.com\n  authorizationUrl: https://comos-portal.com/oauth/authorize\n  tokenUrl: https://comos-portal.com/oauth/token\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n\
  \  pkce:\n  - S256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  metadata: https://comos-portal.com/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://comos-portal.com/.well-known/oauth-protected-resource\n  scopes_ref: scopes/comos-portal-com-scopes.yml\n- type: signature\n  name: node signature\n  description: 'Self-hosted node calls (e.g. federation_node_report_in) are NODE-SIGNED rather than operator-token''d: the node signs the canonical envelope { node_id, nonce, timestamp, route } (OpenAPI description).'\nsso: Enterprise SSO via OIDC (Okta, Azure AD, any provider) — stated on https://comos-portal.com/security\n"
source_yaml_url: https://artifacts.apis.io/comos-portal-com/authentication/comos-portal-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Commerce
- AI Agents
- Operating System
- Federation
- Payments
- Ledger
- Self-Hosted
- E-Commerce
- MCP
---
