---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Openbao Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenBao declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: OpenBao
provider_slug: openbao
scheme_count: 4
schemes:
- description: The canonical way to present a client token. Used by the OpenBao CLI, UI and Go client.
  id: vault-token-header
  in: header
  name: X-Vault-Token
  primary: true
  type: apiKey
- description: Equivalent alternative - Authorization Bearer <token>. Accepted anywhere X-Vault-Token is.
  id: bearer-token
  scheme: bearer
  type: http
- description: The cert auth method authenticates a caller by TLS client certificate at POST /v1/auth/cert/login, exchanging the certificate for a client token. mTLS is an auth METHOD here, not a transport-level alternative to the token - the resulting token still authorizes subsequent calls.
  id: mutual-tls
  type: mutualTLS
- description: The jwt auth method accepts both raw JWTs and a full OIDC login flow. Separately, OpenBao can ACT AS an OIDC provider for third parties via the identity/oidc endpoints, serving its own .well-known/openid-configuration and JWKS from the running instance.
  id: openid-connect
  type: openIdConnect
slug: openbao-authentication
source_filename: openbao-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://openbao.org/docs/api/ ; https://openbao.org/docs/auth/ ; https://openbao.org/docs/concepts/tokens/\ndocs: https://openbao.org/docs/api/\nname: OpenBao authentication\nsummary: >-\n  OpenBao is token-authenticated. Once an instance is unsealed, almost every operation requires a\n  client token. The token is sent either in the X-Vault-Token request header or as an Authorization\n  header using the Bearer <token> scheme. There is no OAuth 2.0 authorization-code flow for the\n  OpenBao API itself and therefore no scope surface - authorization is expressed as ACL policies\n  attached to the token, not as OAuth scopes. Tokens are obtained from an auth method: each auth\n  method exposes one or more UNAUTHENTICATED login endpoints, which are the only routes reachable\n  with no credential at all (alongside sys/health, sys/seal-status and the unseal/generate-root\n  attempt endpoints).\nschemes:\n- id: vault-token-header\n\
  \  type: apiKey\n  in: header\n  name: X-Vault-Token\n  description: The canonical way to present a client token. Used by the OpenBao CLI, UI and Go client.\n  primary: true\n- id: bearer-token\n  type: http\n  scheme: bearer\n  description: Equivalent alternative - Authorization Bearer <token>. Accepted anywhere X-Vault-Token is.\n- id: mutual-tls\n  type: mutualTLS\n  description: >-\n    The cert auth method authenticates a caller by TLS client certificate at POST /v1/auth/cert/login,\n    exchanging the certificate for a client token. mTLS is an auth METHOD here, not a transport-level\n    alternative to the token - the resulting token still authorizes subsequent calls.\n- id: openid-connect\n  type: openIdConnect\n  description: >-\n    The jwt auth method accepts both raw JWTs and a full OIDC login flow. Separately, OpenBao can ACT\n    AS an OIDC provider for third parties via the identity/oidc endpoints, serving its own\n    .well-known/openid-configuration and JWKS from the running\
  \ instance.\nauth_methods:\n- id: token\n  path: auth/token\n  note: Built-in. Tokens created directly, with TTLs, renewal, orphaning and use-limits.\n- id: approle\n  path: auth/approle\n  note: RoleID + SecretID, intended for machines and CI.\n- id: cert\n  path: auth/cert\n  note: TLS client certificates.\n- id: jwt\n  path: auth/jwt\n  note: JWT and OIDC. Supports CEL-based roles.\n- id: kerberos\n  path: auth/kerberos\n- id: kubernetes\n  path: auth/kubernetes\n  note: Service-account token review against the cluster API.\n- id: ldap\n  path: auth/ldap\n- id: radius\n  path: auth/radius\n- id: userpass\n  path: auth/userpass\nauthorization_model:\n  style: acl-policies\n  description: >-\n    Capabilities (create, read, update, patch, delete, list, sudo, deny) are granted per path glob by\n    an ACL policy written in HCL or JSON and managed at sys/policies/acl/:name. Policies attach to\n    tokens and to identity entities/groups. There are no OAuth scopes; sys/capabilities-self reports\n\
  \    what the calling token may do on a path.\n  sudo_paths: Some root-protected paths additionally require the sudo capability; the generated OpenAPI marks them with x-vault-sudo.\n  namespaces: Requests are scoped to a namespace by the X-Vault-Namespace header or an equivalent full path.\nmfa:\n  supported: true\n  note: Login MFA (TOTP, Duo, Okta, PingID) is configured under identity/mfa and enforced by login-enforcement objects.\nresponse_wrapping:\n  supported: true\n  header: X-Vault-Wrap-TTL\n  note: >-\n    Any response can be wrapped into a single-use token by sending X-Vault-Wrap-TTL. The caller\n    receives wrap_info instead of the payload and must unwrap at sys/wrapping/unwrap. This is\n    OpenBao's secure-introduction primitive and is unusual enough to be worth naming explicitly.\nunauthenticated_endpoints:\n- /v1/sys/health\n- /v1/sys/seal-status\n- /v1/auth/:method/login/... (per auth method)\n- /v1/sys/unseal\n- /v1/sys/generate-root/attempt\n- /v1/sys/generate-root/update\n\
  notes:\n- The X-Vault-* header prefix is retained deliberately for API compatibility with HashiCorp Vault, which OpenBao was forked from.\n- The X-Vault-Request header must be present on requests routed through an OpenBao Proxy configured with require_request_header; the CLI and Go SDK always set it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openbao/refs/heads/main/authentication/openbao-authentication.yml
summary_line: 4 schemes
tags:
- Secrets Management
- Security
- Identity and Access Management
- Encryption
- Certificates
- PKI
- Key Management
- Open-Source
- Self-Hosted
- Linux Foundation
- DevOps
- Infrastructure
---
