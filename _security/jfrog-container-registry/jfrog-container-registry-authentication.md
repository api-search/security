---
api_key_in: []
auth_types: []
description: Authentication profile for the JFrog Platform surface that serves JFrog Container Registry. DERIVED FROM DOCS, NOT FROM A SPEC — JFrog publishes no downloadable OpenAPI document, so no securitySchemes block was available to read. Every scheme below is stated on the JFrog documentation page cited on it.
kind: authentication
layout: security
method: searched
name: Jfrog Container Registry Authentication
name_suffix: Authentication
oauth_flows: []
overview: JFrog Container Registry declares 9 security scheme(s) across its OpenAPI definitions.
provider_name: JFrog Container Registry
provider_slug: jfrog-container-registry
scheme_count: 9
schemes:
- description: Scoped access tokens are the platform's primary API credential. Since Artifactory 7.21.1 all access tokens are scoped tokens; REST API access is granted by default and additional group memberships or roles are attached via the scope string.
  docs: https://docs.jfrog.com/administration/docs/access-tokens
  features:
  - expiring tokens (revocable-expiry and persistency thresholds)
  - refreshable tokens
  - admin tokens
  - project-admin tokens
  - reference tokens (short opaque token usable as a basic-auth password)
  header: 'Authorization: Bearer <access token>'
  id: bearer-access-token
  name: JFrog Access Token
  primary: true
  scheme: bearer
  token_endpoint: POST https://<JFrogPlatformURL>/access/api/v1/tokens
  type: http
- description: Username plus password, or username plus a reference token, for clients that only support basic auth (certain dependency managers). The same username used when the reference token was created must be supplied.
  docs: https://docs.jfrog.com/administration/docs/access-tokens
  id: basic
  name: Basic authentication
  scheme: basic
  type: http
- description: Container clients authenticate against the registry token endpoint before push/pull. This is the scheme a container runtime actually uses against JFrog Container Registry.
  docs: https://docs.jfrog.com/artifactory/docs/docker-repositories
  endpoint: https://<JFrogPlatformURL>/artifactory/api/docker/<REPO_NAME>/<V1|V2>/auth
  id: docker-registry-token
  name: Docker/OCI registry token auth
  type: oauth2-like
- description: Exchange an external OIDC identity token (for example a GitHub Actions workload identity) for a JFrog access token — no long-lived secret in CI.
  docs:
  - https://docs.jfrog.com/integrations/docs/jf-exchange-oidc-token
  - https://docs.jfrog.com/integrations/docs/github-actions-oidc-authentication
  id: oidc
  name: OIDC token exchange
  type: openIdConnect
- description: The remote JFrog MCP Server authorizes MCP clients over OAuth rather than API keys; the client opens a browser consent window on first connect.
  docs: https://github.com/jfrog/jfrog-mcp-server
  id: oauth-mcp
  name: OAuth (JFrog MCP Server)
  type: oauth2
- docs:
  - https://docs.jfrog.com/artifactory/docs/authentication
  - https://docs.jfrog.com/administration/docs/mtls-authentication-in-jfrog-saas
  id: mtls
  name: Mutual TLS client certificates
  type: mutualTLS
- description: Supported from Artifactory 4.4 for the Artifactory SSH URL (ssh://[host]:[port]). NOT supported with external package managers and build tools (Maven, Gradle, npm, Docker, Go, NuGet) or with `jf rt curl`.
  docs: https://docs.jfrog.com/artifactory/docs/authentication
  id: ssh-rsa
  name: SSH / RSA key authentication
  type: other
- description: Interactive CLI login that opens a browser session against the platform.
  docs: https://docs.jfrog.com/integrations/docs/authenticating-via-the-cli
  id: browser-login
  name: Browser login (`jf login`)
  type: other
- description: CLI credentials supplied through environment variables for CI use.
  docs: https://docs.jfrog.com/integrations/docs/authenticating-via-the-cli
  id: env-var
  name: Environment-variable authentication
  type: other
slug: jfrog-container-registry-authentication
source_filename: jfrog-container-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: JFrog Container Registry\nproviderId: jfrog-container-registry\ngenerated: '2026-08-29'\nmodified: '2026-08-29'\nmethod: searched\nsource: https://docs.jfrog.com/integrations/docs/authenticating-via-the-cli\ndocs:\n  - https://docs.jfrog.com/administration/docs/jfrog-authentication-and-token-management-overview\n  - https://docs.jfrog.com/administration/docs/access-tokens\n  - https://docs.jfrog.com/artifactory/docs/authentication\n  - https://docs.jfrog.com/administration/docs/authentication-providers\n  - https://docs.jfrog.com/artifactory/docs/docker-repositories\ndescription: >-\n  Authentication profile for the JFrog Platform surface that serves JFrog Container Registry.\n  DERIVED FROM DOCS, NOT FROM A SPEC — JFrog publishes no downloadable OpenAPI document, so no\n  securitySchemes block was available to read. Every scheme below is stated on the JFrog\n  documentation page cited on it.\n\
  schemes:\n  - id: bearer-access-token\n    type: http\n    scheme: bearer\n    primary: true\n    name: JFrog Access Token\n    description: >-\n      Scoped access tokens are the platform's primary API credential. Since Artifactory 7.21.1\n      all access tokens are scoped tokens; REST API access is granted by default and additional\n      group memberships or roles are attached via the scope string.\n    header: 'Authorization: Bearer <access token>'\n    token_endpoint: 'POST https://<JFrogPlatformURL>/access/api/v1/tokens'\n    docs: https://docs.jfrog.com/administration/docs/access-tokens\n    features:\n      - expiring tokens (revocable-expiry and persistency thresholds)\n      - refreshable tokens\n      - admin tokens\n      - project-admin tokens\n      - reference tokens (short opaque token usable as a basic-auth password)\n  - id: basic\n    type: http\n    scheme: basic\n    name: Basic authentication\n    description: >-\n      Username plus password, or username plus a\
  \ reference token, for clients that only support\n      basic auth (certain dependency managers). The same username used when the reference token\n      was created must be supplied.\n    docs: https://docs.jfrog.com/administration/docs/access-tokens\n  - id: docker-registry-token\n    type: oauth2-like\n    name: Docker/OCI registry token auth\n    description: >-\n      Container clients authenticate against the registry token endpoint before push/pull.\n      This is the scheme a container runtime actually uses against JFrog Container Registry.\n    endpoint: 'https://<JFrogPlatformURL>/artifactory/api/docker/<REPO_NAME>/<V1|V2>/auth'\n    docs: https://docs.jfrog.com/artifactory/docs/docker-repositories\n  - id: oidc\n    type: openIdConnect\n    name: OIDC token exchange\n    description: >-\n      Exchange an external OIDC identity token (for example a GitHub Actions workload identity)\n      for a JFrog access token — no long-lived secret in CI.\n    docs:\n      - https://docs.jfrog.com/integrations/docs/jf-exchange-oidc-token\n\
  \      - https://docs.jfrog.com/integrations/docs/github-actions-oidc-authentication\n  - id: oauth-mcp\n    type: oauth2\n    name: OAuth (JFrog MCP Server)\n    description: >-\n      The remote JFrog MCP Server authorizes MCP clients over OAuth rather than API keys; the\n      client opens a browser consent window on first connect.\n    docs: https://github.com/jfrog/jfrog-mcp-server\n  - id: mtls\n    type: mutualTLS\n    name: Mutual TLS client certificates\n    docs:\n      - https://docs.jfrog.com/artifactory/docs/authentication\n      - https://docs.jfrog.com/administration/docs/mtls-authentication-in-jfrog-saas\n  - id: ssh-rsa\n    type: other\n    name: SSH / RSA key authentication\n    description: >-\n      Supported from Artifactory 4.4 for the Artifactory SSH URL (ssh://[host]:[port]).\n      NOT supported with external package managers and build tools (Maven, Gradle, npm, Docker,\n      Go, NuGet) or with `jf rt curl`.\n    docs: https://docs.jfrog.com/artifactory/docs/authentication\n\
  \  - id: browser-login\n    type: other\n    name: Browser login (`jf login`)\n    description: Interactive CLI login that opens a browser session against the platform.\n    docs: https://docs.jfrog.com/integrations/docs/authenticating-via-the-cli\n  - id: env-var\n    type: other\n    name: Environment-variable authentication\n    description: CLI credentials supplied through environment variables for CI use.\n    docs: https://docs.jfrog.com/integrations/docs/authenticating-via-the-cli\nidentity_providers:\n  - SAML 2.0 SSO\n  - LDAP\n  - Multi-factor authentication (MFA) for platform login\n  - SCIM 2.0 user/group provisioning (Enterprise X / Enterprise+)\ndocs_identity_providers: https://docs.jfrog.com/administration/docs/authentication-providers\nnotes:\n  - >-\n    Artifactory API Keys are being retired in favour of scoped access tokens; the Artifactory\n    release notes flag \"important changes to authentication\" for self-managed versions 7.98.7\n    and above (https://docs.jfrog.com/releases/docs/artifactory-self-managed-releases).\n\
  \  - >-\n    Every credential is tenant-scoped. There is no shared public API host to authenticate\n    against — the host is the customer's own JFrog Platform Deployment.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jfrog-container-registry/refs/heads/main/authentication/jfrog-container-registry-authentication.yml
summary_line: 9 schemes
tags:
- Container Images
- Containers
- Docker
- Helm
- JFrog
- Registry
---
