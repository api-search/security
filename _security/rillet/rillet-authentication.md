---
api_key_in:
- header
api_specs:
- filename: rillet-accounting-api-openapi.json
  format: json
  label: Rillet Accounting API
  slug: rillet-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rillet/refs/heads/main/openapi/rillet-accounting-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rillet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Rillet secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Rillet
provider_slug: rillet
scheme_count: 2
schemes:
- description: 'API keys are passed as a Bearer token in the Authorization header (Authorization: Bearer <api_key>). Keys are managed on the Organization Settings page. This is the primary auth for direct API access.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rillet-accounting-api-openapi.json
  type: http
- description: OAuth 2.0 authorization-code flow (PKCE S256) used for the remote MCP server and third-party connectors. Discovered via RFC 8414 metadata at /.well-known/oauth-authorization-server and RFC 9728 protected-resource metadata at /.well-known/oauth-protected-resource. Access tokens may be mutual-TLS or DPoP sender-constrained.
  flows:
  - authorizationUrl: https://api.rillet.com/oauth2/authorize
    flow: authorizationCode
    introspectionUrl: https://api.rillet.com/oauth2/introspect
    jwksUri: https://api.rillet.com/oauth2/jwks
    pkce: S256
    revocationUrl: https://api.rillet.com/oauth2/revoke
    scopes:
      read: Read access to Rillet resources
      write: Write access to Rillet resources
    tokenUrl: https://api.rillet.com/oauth2/token
  name: oauth2
  sender_constrained:
    dpop: true
    mtls: true
  sources:
  - well-known/rillet-oauth-authorization-server.json
  - well-known/rillet-oauth-protected-resource.json
  type: oauth2
slug: rillet-authentication
source_filename: rillet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/rillet-accounting-api-openapi.json\ndocs: https://docs.api.rillet.com/docs/getting-started\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API keys are passed as a Bearer token in the Authorization header\n    (Authorization: Bearer <api_key>). Keys are managed on the Organization\n    Settings page. This is the primary auth for direct API access.\n  sources:\n  - openapi/rillet-accounting-api-openapi.json\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code flow (PKCE S256) used for the remote MCP\n    server and third-party connectors. Discovered via RFC 8414 metadata at\n    /.well-known/oauth-authorization-server and RFC 9728 protected-resource\n    metadata at /.well-known/oauth-protected-resource. Access tokens may be\n    mutual-TLS\
  \ or DPoP sender-constrained.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.rillet.com/oauth2/authorize\n    tokenUrl: https://api.rillet.com/oauth2/token\n    revocationUrl: https://api.rillet.com/oauth2/revoke\n    introspectionUrl: https://api.rillet.com/oauth2/introspect\n    jwksUri: https://api.rillet.com/oauth2/jwks\n    pkce: S256\n    scopes:\n      read: Read access to Rillet resources\n      write: Write access to Rillet resources\n  sender_constrained:\n    mtls: true\n    dpop: true\n  sources:\n  - well-known/rillet-oauth-authorization-server.json\n  - well-known/rillet-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rillet/refs/heads/main/authentication/rillet-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Fintech
- ERP
- Accounting
- Finance
- General Ledger
- Accounts Receivable
- Accounts Payable
- Invoicing
- SaaS
---
