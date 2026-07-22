---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Moderne Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moderne secures its APIs with http, oauth2, openIdConnect, and saml across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Moderne
provider_slug: moderne
scheme_count: 2
schemes:
- description: 'Personal access tokens authenticate all programmatic access — the GraphQL API (https://api.app.moderne.io/graphql), the remote MCP server, and the Moderne CLI. Sent as `Authorization: Bearer <token>`. Tokens carry the same permissions as the issuing account and are created in Account Settings > Access Tokens with a configurable expiry (7/30/90 days, custom, or no expiration, subject to an org-configured maximum). CLI tokens use the `mat-` prefix.'
  extra_headers:
  - name: X-Moderne-Platform-Version
    note: Required while SaaS v1 and v2 run in parallel (API and remote MCP).
    value: v2
  header:
    format: Bearer <token>
    name: Authorization
  name: PersonalAccessToken
  scheme: bearer
  token_endpoint_ui: https://app.moderne.io/settings/access-token
  type: http
- description: Interactive human authentication to the Moderne Platform is via SSO brokered by a dedicated Keycloak server acting as an identity broker to the customer Identity Provider. Supports SAML, OIDC, and social logins (Google, GitHub). Browser flow uses PKCE and issues an opaque JWT validated server-side against Keycloak. IdP claims (email, firstName, lastName, admin role) are mapped into Keycloak on each authentication.
  flow: authorization-code-pkce
  identity_broker: Keycloak
  name: SSO
  protocols:
  - OIDC
  - SAML
  type: openIdConnect
slug: moderne-authentication
source_filename: moderne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.moderne.io/administrator-documentation/moderne-platform/references/authentication\ndocs: https://docs.moderne.io/user-documentation/moderne-platform/how-to-guides/create-api-access-tokens\nsummary:\n  types: [http, oauth2, openIdConnect, saml]\n  api_access: bearer-personal-access-token\n  sso: [SAML, OIDC, social-login]\n  identity_broker: Keycloak\nschemes:\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  description: >-\n    Personal access tokens authenticate all programmatic access — the GraphQL API\n    (https://api.app.moderne.io/graphql), the remote MCP server, and the Moderne\n    CLI. Sent as `Authorization: Bearer <token>`. Tokens carry the same permissions\n    as the issuing account and are created in Account Settings > Access Tokens with\n    a configurable expiry (7/30/90 days, custom, or no expiration, subject to an\n    org-configured maximum). CLI tokens use the `mat-` prefix.\n\
  \  token_endpoint_ui: https://app.moderne.io/settings/access-token\n  header:\n    name: Authorization\n    format: Bearer <token>\n  extra_headers:\n  - name: X-Moderne-Platform-Version\n    value: v2\n    note: Required while SaaS v1 and v2 run in parallel (API and remote MCP).\n- name: SSO\n  type: openIdConnect\n  description: >-\n    Interactive human authentication to the Moderne Platform is via SSO brokered\n    by a dedicated Keycloak server acting as an identity broker to the customer\n    Identity Provider. Supports SAML, OIDC, and social logins (Google, GitHub).\n    Browser flow uses PKCE and issues an opaque JWT validated server-side against\n    Keycloak. IdP claims (email, firstName, lastName, admin role) are mapped into\n    Keycloak on each authentication.\n  protocols: [OIDC, SAML]\n  flow: authorization-code-pkce\n  identity_broker: Keycloak\nnotes:\n- The GraphQL API and remote MCP server share the same personal-access-token auth.\n- SCM access tokens (separate) are\
  \ required to commit results back to source control.\n- Company has no OpenAPI; auth profile derived from published documentation (searched).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moderne/refs/heads/main/authentication/moderne-authentication.yml
summary_line: http/oauth2/openIdConnect/saml · 2 schemes
tags:
- Company
- Developer Tools
- Code Transformation
- Automated Refactoring
- Code Migration
- Security Patching
- OpenRewrite
- Static Analysis
- Code Governance
- DevOps
- GraphQL
- AI Agents
- MCP
---
