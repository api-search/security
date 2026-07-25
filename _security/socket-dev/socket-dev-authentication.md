---
api_key_in: []
api_specs:
- filename: socket-dev-alerts-api-openapi.yml
  format: yaml
  label: Socket alerts API
  slug: socket-dev-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-alerts-api-openapi.yml
- filename: socket-dev-api-tokens-api-openapi.yml
  format: yaml
  label: Socket api-tokens API
  slug: socket-dev-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-api-tokens-api-openapi.yml
- filename: socket-dev-audit-log-api-openapi.yml
  format: yaml
  label: Socket audit-log API
  slug: socket-dev-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-audit-log-api-openapi.yml
- filename: socket-dev-dependencies-api-openapi.yml
  format: yaml
  label: Socket dependencies API
  slug: socket-dev-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-dependencies-api-openapi.yml
- filename: socket-dev-diff-scans-api-openapi.yml
  format: yaml
  label: Socket diff-scans API
  slug: socket-dev-diff-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-diff-scans-api-openapi.yml
- filename: socket-dev-fixes-api-openapi.yml
  format: yaml
  label: Socket fixes API
  slug: socket-dev-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-fixes-api-openapi.yml
- filename: socket-dev-full-scans-api-openapi.yml
  format: yaml
  label: Socket full-scans API
  slug: socket-dev-full-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-full-scans-api-openapi.yml
- filename: socket-dev-license-policy-api-openapi.yml
  format: yaml
  label: Socket license-policy API
  slug: socket-dev-license-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-license-policy-api-openapi.yml
- filename: socket-dev-metadata-api-openapi.yml
  format: yaml
  label: Socket metadata API
  slug: socket-dev-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-metadata-api-openapi.yml
- filename: socket-dev-org-settings-api-openapi.yml
  format: yaml
  label: Socket org-settings API
  slug: socket-dev-org-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-org-settings-api-openapi.yml
- filename: socket-dev-org-snapshots-api-openapi.yml
  format: yaml
  label: Socket org-snapshots API
  slug: socket-dev-org-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-org-snapshots-api-openapi.yml
- filename: socket-dev-packages-api-openapi.yml
  format: yaml
  label: Socket packages API
  slug: socket-dev-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-packages-api-openapi.yml
- filename: socket-dev-repo-labels-api-openapi.yml
  format: yaml
  label: Socket repo-labels API
  slug: socket-dev-repo-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-repo-labels-api-openapi.yml
- filename: socket-dev-repos-api-openapi.yml
  format: yaml
  label: Socket repos API
  slug: socket-dev-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-repos-api-openapi.yml
- filename: socket-dev-security-policy-api-openapi.yml
  format: yaml
  label: Socket security-policy API
  slug: socket-dev-security-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-security-policy-api-openapi.yml
- filename: socket-dev-telemetry-api-openapi.yml
  format: yaml
  label: Socket telemetry API
  slug: socket-dev-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-telemetry-api-openapi.yml
- filename: socket-dev-threat-feed-api-openapi.yml
  format: yaml
  label: Socket threat-feed API
  slug: socket-dev-threat-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-threat-feed-api-openapi.yml
- filename: socket-dev-triage-api-openapi.yml
  format: yaml
  label: Socket triage API
  slug: socket-dev-triage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-triage-api-openapi.yml
- filename: socket-dev-webhooks-api-openapi.yml
  format: yaml
  label: Socket webhooks API
  slug: socket-dev-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dev-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Socket Dev Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Socket secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Socket
provider_slug: socket-dev
scheme_count: 3
schemes:
- description: Organization Tokens can be passed as a Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/socket-alerts-api-openapi.yml
  - openapi/socket-api-tokens-api-openapi.yml
  - openapi/socket-audit-log-api-openapi.yml
  - openapi/socket-dependencies-api-openapi.yml
  - openapi/socket-diff-scans-api-openapi.yml
  - openapi/socket-fixes-api-openapi.yml
  - openapi/socket-full-scans-api-openapi.yml
  - openapi/socket-metadata-api-openapi.yml
  - openapi/socket-org-settings-api-openapi.yml
  - openapi/socket-org-snapshots-api-openapi.yml
  - openapi/socket-packages-api-openapi.yml
  - openapi/socket-repos-api-openapi.yml
  - openapi/socket-threat-feed-api-openapi.yml
  - openapi/socket-triage-api-openapi.yml
  - openapi/socket-webhooks-api-openapi.yml
  type: http
- description: Organization Tokens can be passed as the user field in basic auth
  name: basicAuth
  scheme: basic
  sources:
  - openapi/socket-alerts-api-openapi.yml
  - openapi/socket-api-tokens-api-openapi.yml
  - openapi/socket-audit-log-api-openapi.yml
  - openapi/socket-dependencies-api-openapi.yml
  - openapi/socket-diff-scans-api-openapi.yml
  - openapi/socket-fixes-api-openapi.yml
  - openapi/socket-full-scans-api-openapi.yml
  - openapi/socket-metadata-api-openapi.yml
  - openapi/socket-org-settings-api-openapi.yml
  - openapi/socket-org-snapshots-api-openapi.yml
  - openapi/socket-packages-api-openapi.yml
  - openapi/socket-repos-api-openapi.yml
  - openapi/socket-threat-feed-api-openapi.yml
  - openapi/socket-triage-api-openapi.yml
  - openapi/socket-webhooks-api-openapi.yml
  type: http
- description: 'Live OAuth 2.0 authorization server advertised at api.socket.dev/.well-known/oauth-authorization-server (RFC 8414). Client classes: customer_user_delegated (authorization_code + refresh_token) and customer_machine_to_machine (client_credentials).'
  flows:
  - authorizationUrl: https://api.socket.dev/v1/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    scope_count: 97
    tokenUrl: https://api.socket.dev/v1/oauth2/token
  - flow: clientCredentials
    scope_count: 97
    tokenUrl: https://api.socket.dev/v1/oauth2/token
  name: OAuth2
  scopes: scopes/socket-dev-scopes.yml
  sources:
  - well-known/socket-dev-oauth-authorization-server.json
  type: oauth2
slug: socket-dev-authentication
source_filename: socket-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/*-openapi.yml + well-known/socket-dev-oauth-authorization-server.json (RFC 8414 metadata)\ndocs: https://docs.socket.dev/reference/authentication-types\nnote: >-\n  The OpenAPI specs declare only http bearer + basic (Organization tokens). A live probe of\n  api.socket.dev/.well-known/oauth-authorization-server additionally reveals a full OAuth 2.0\n  authorization server (authorization_code + client_credentials + refresh_token, PKCE S256,\n  97 scopes) — added below as the oauth2 scheme. Scope list in scopes/socket-dev-scopes.yml.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Organization Tokens can be passed as a Bearer token\n  sources:\n  - openapi/socket-alerts-api-openapi.yml\n  - openapi/socket-api-tokens-api-openapi.yml\n  - openapi/socket-audit-log-api-openapi.yml\n  - openapi/socket-dependencies-api-openapi.yml\n\
  \  - openapi/socket-diff-scans-api-openapi.yml\n  - openapi/socket-fixes-api-openapi.yml\n  - openapi/socket-full-scans-api-openapi.yml\n  - openapi/socket-metadata-api-openapi.yml\n  - openapi/socket-org-settings-api-openapi.yml\n  - openapi/socket-org-snapshots-api-openapi.yml\n  - openapi/socket-packages-api-openapi.yml\n  - openapi/socket-repos-api-openapi.yml\n  - openapi/socket-threat-feed-api-openapi.yml\n  - openapi/socket-triage-api-openapi.yml\n  - openapi/socket-webhooks-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Organization Tokens can be passed as the user field in basic auth\n  sources:\n  - openapi/socket-alerts-api-openapi.yml\n  - openapi/socket-api-tokens-api-openapi.yml\n  - openapi/socket-audit-log-api-openapi.yml\n  - openapi/socket-dependencies-api-openapi.yml\n  - openapi/socket-diff-scans-api-openapi.yml\n  - openapi/socket-fixes-api-openapi.yml\n  - openapi/socket-full-scans-api-openapi.yml\n  - openapi/socket-metadata-api-openapi.yml\n\
  \  - openapi/socket-org-settings-api-openapi.yml\n  - openapi/socket-org-snapshots-api-openapi.yml\n  - openapi/socket-packages-api-openapi.yml\n  - openapi/socket-repos-api-openapi.yml\n  - openapi/socket-threat-feed-api-openapi.yml\n  - openapi/socket-triage-api-openapi.yml\n  - openapi/socket-webhooks-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Live OAuth 2.0 authorization server advertised at\n    api.socket.dev/.well-known/oauth-authorization-server (RFC 8414). Client classes:\n    customer_user_delegated (authorization_code + refresh_token) and\n    customer_machine_to_machine (client_credentials).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.socket.dev/v1/oauth2/authorize\n    tokenUrl: https://api.socket.dev/v1/oauth2/token\n    pkce: S256\n    scope_count: 97\n  - flow: clientCredentials\n    tokenUrl: https://api.socket.dev/v1/oauth2/token\n    scope_count: 97\n  scopes: scopes/socket-dev-scopes.yml\n  sources:\n  - well-known/socket-dev-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/authentication/socket-dev-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Supply Chain Security
- Open Source Security
- Software Composition Analysis
- SCA
- Malware Detection
- Dependency Scanning
- SBOM
- npm
- PyPI
- Go
- Maven
- Cargo
- NuGet
- RubyGems
- Developer Security
---
