---
api_key_in: []
api_specs:
- filename: upwind-security-management-v2-openapi.yml
  format: yaml
  label: Upwind Management REST API v2
  slug: management-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/openapi/upwind-security-management-v2-openapi.yml
- filename: upwind-security-management-v1-openapi.yml
  format: yaml
  label: Upwind Management REST API v1
  slug: management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/openapi/upwind-security-management-v1-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Upwind Security Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Upwind Security secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Upwind Security
provider_slug: upwind-security
scheme_count: 1
schemes:
- description: All Management REST API requests authenticate with OAuth 2.0 client_credentials. Generate a Client ID/Secret in the Upwind console (Settings -> Credentials, "API" credential type), then exchange them at the token endpoint with an audience matching the regional API base URL. Tokens are JWTs, valid 24 hours, and region-locked (a US-audience token will not work against the EU endpoint).
  flows:
    clientCredentials:
      audiences:
        eu: https://api.eu.upwind.io
        me: https://api.me.upwind.io
        us: https://api.upwind.io
      tokenUrl: https://auth.upwind.io/oauth/token
  identity_providers:
  - issuer: https://auth.upwind.io/ (Auth0) — API token endpoint
  - issuer: https://oauth.upwind.io/realms/upwind (Keycloak) — platform/MCP OIDC discovery on api.upwind.io and mcp.upwind.io
  name: OAuth2ClientCredentials
  rbac: API credentials carry an RBAC scope (which resources — clusters, cloud accounts, environments — the token may access) and roles. Credentials can never exceed the access level of the member who created them, and tokens inherit the credential's permissions.
  type: oauth2
slug: upwind-security-authentication
source_filename: upwind-security-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.upwind.io/restapi/v2/introduction
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.upwind.io/restapi/v2/introduction\nsources:\n  - https://docs.upwind.io/restapi/v2/introduction\n  - https://docs.upwind.io/settings/credentials\n  - https://api.upwind.io/.well-known/openid-configuration\n  - https://auth.upwind.io/.well-known/openid-configuration\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_format: JWT (RFC 7519) bearer access tokens\n  token_lifetime: 24h\n  header: 'Authorization: Bearer <access_token>'\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    description: >-\n      All Management REST API requests authenticate with OAuth 2.0\n      client_credentials. Generate a Client ID/Secret in the Upwind console\n      (Settings -> Credentials, \"API\" credential type), then exchange them at\n      the token endpoint with an audience matching the regional API base URL.\n      Tokens are JWTs, valid 24 hours, and region-locked (a US-audience token\n\
  \      will not work against the EU endpoint).\n    flows:\n      clientCredentials:\n        tokenUrl: https://auth.upwind.io/oauth/token\n        audiences:\n          us: https://api.upwind.io\n          eu: https://api.eu.upwind.io\n          me: https://api.me.upwind.io\n    rbac: >-\n      API credentials carry an RBAC scope (which resources — clusters, cloud\n      accounts, environments — the token may access) and roles. Credentials\n      can never exceed the access level of the member who created them, and\n      tokens inherit the credential's permissions.\n    identity_providers:\n      - issuer: https://auth.upwind.io/ (Auth0) — API token endpoint\n      - issuer: https://oauth.upwind.io/realms/upwind (Keycloak) — platform/MCP OIDC discovery on api.upwind.io and mcp.upwind.io\ncredential_types:\n  - Cloud account (connect AWS, GCP, Azure, Oracle)\n  - Sensor (Helm/Bash sensor deployment)\n  - API (Management REST API access)\n  - Integration (third-party services such as Slack,\
  \ Kubernetes Audit Logs, GitHub Actions)\nopenapi_note: >-\n  The published OpenAPI 3.1 specs (v1, v2) do not declare\n  components.securitySchemes; the auth contract above is documented in the\n  API introduction and credentials docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/authentication/upwind-security-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cybersecurity
- Cloud Security
- CNAPP
- Runtime Security
- Vulnerability Management
- API Security
- Kubernetes
---
