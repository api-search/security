---
api_key_in:
- header
api_specs:
- filename: venafi-certificate-manager-saas-openapi.yml
  format: yaml
  label: Certificate Manager - SaaS API (Venafi Control Plane)
  slug: certificate-manager-saas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/openapi/venafi-certificate-manager-saas-openapi.yml
- filename: venafi-trust-protection-foundation-websdk-openapi.yml
  format: yaml
  label: Trust Protection Foundation WebSDK (Venafi Trust Protection Platform)
  slug: trust-protection-foundation-websdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/openapi/venafi-trust-protection-foundation-websdk-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Venafi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Venafi secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Venafi
provider_slug: venafi
scheme_count: 4
schemes:
- api: Certificate Manager - SaaS API
  description: 'User API key, generated at account registration and readable from the console (avatar > Preferences > API Keys) or via `vcert getcred --email <address>`. Sent on every call alongside Content-Type: application/json. Keys rotate with an active/pending pair — the pending (previous) key stays valid until its validity period ends or it is deleted.'
  docs: https://docs.venafi.cloud/api/obtaining-api-key/
  in: header
  name: tppl-api-key
  parameter: tppl-api-key
  sources:
  - openapi/venafi-certificate-manager-saas-openapi.yml
  type: apiKey
- api: Certificate Manager - SaaS API
  description: 'Service-account credential scheme declared in the SaaS contract as an apiKey header named "service-account". NOTE — the provider''s own documentation states that a service account access token is sent in the standard `Authorization: Bearer` header, not in a `service-account` header; the contract and the docs disagree and this is recorded as published rather than reconciled. Service accounts are created via POST /v1/serviceaccounts and their available scopes read from GET /v1/serviceaccounts/scopes.'
  docs: https://docs.venafi.cloud/api/obtaining-api-key/
  in: header
  name: service-account
  parameter: service-account
  sources:
  - openapi/venafi-certificate-manager-saas-openapi.yml
  type: apiKey
- api: Trust Protection Foundation WebSDK
  description: OAuth 2.0 bearer access token issued by the customer's own Trust Protection Foundation authorization server. Obtained from POST /vedauth/authorize/oauth (authorization code), /device, /jwt, /certificate or /integrated; refreshed with POST /vedauth/authorize/token and revoked with DELETE /vedauth/revoke/token. Every operation declares its required scope (see scopes/venafi-scopes.yml).
  docs: https://docs.venafi.com/Docs/currentSDK/TopNav/Content/SDK/AuthSDK/t-SDKa-Setup-OAuth.php
  name: AccessToken
  scheme: bearer
  sources:
  - openapi/venafi-trust-protection-foundation-websdk-openapi.yml
  type: http
- api: Certificate Manager - SaaS ACMEv2 server
  description: ACME clients authenticate to the Certificate Manager - SaaS ACMEv2 server with External Account Binding (EAB) per RFC 8555 §7.3.4. Domain-ownership challenges (HTTP-01, DNS-01, TLS-ALPN-01) are not used; issuance is governed by the configured application and request policy instead.
  docs: https://docs.venafi.cloud/vaas/configurations/acme-server-overview/
  name: acme-external-account-binding
  sources:
  - https://docs.venafi.cloud/vaas/configurations/acme-server-overview/
  type: other
slug: venafi-authentication
source_filename: venafi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: openapi/venafi-certificate-manager-saas-openapi.yml,\n  openapi/venafi-trust-protection-foundation-websdk-openapi.yml\ndocs: https://docs.venafi.cloud/api/obtaining-api-key/\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: tppl-api-key\n  type: apiKey\n  in: header\n  parameter: tppl-api-key\n  api: Certificate Manager - SaaS API\n  description: 'User API key, generated at account registration and readable from the console\n    (avatar > Preferences > API Keys) or via `vcert getcred --email <address>`. Sent on every\n    call alongside Content-Type: application/json. Keys rotate with an active/pending pair — the\n    pending (previous) key stays valid until its validity period ends or it is deleted.'\n  docs: https://docs.venafi.cloud/api/obtaining-api-key/\n  sources:\n  - openapi/venafi-certificate-manager-saas-openapi.yml\n- name: service-account\n  type: apiKey\n  in: header\n\
  \  parameter: service-account\n  api: Certificate Manager - SaaS API\n  description: 'Service-account credential scheme declared in the SaaS contract as an apiKey\n    header named \"service-account\". NOTE — the provider''s own documentation states that a\n    service account access token is sent in the standard `Authorization: Bearer` header, not in a\n    `service-account` header; the contract and the docs disagree and this is recorded as\n    published rather than reconciled. Service accounts are created via POST /v1/serviceaccounts\n    and their available scopes read from GET /v1/serviceaccounts/scopes.'\n  docs: https://docs.venafi.cloud/api/obtaining-api-key/\n  sources:\n  - openapi/venafi-certificate-manager-saas-openapi.yml\n- name: AccessToken\n  type: http\n  scheme: bearer\n  api: Trust Protection Foundation WebSDK\n  description: OAuth 2.0 bearer access token issued by the customer's own Trust Protection\n    Foundation authorization server. Obtained from POST /vedauth/authorize/oauth\
  \ (authorization\n    code), /device, /jwt, /certificate or /integrated; refreshed with POST /vedauth/authorize/token\n    and revoked with DELETE /vedauth/revoke/token. Every operation declares its required scope\n    (see scopes/venafi-scopes.yml).\n  docs: https://docs.venafi.com/Docs/currentSDK/TopNav/Content/SDK/AuthSDK/t-SDKa-Setup-OAuth.php\n  sources:\n  - openapi/venafi-trust-protection-foundation-websdk-openapi.yml\n- name: acme-external-account-binding\n  type: other\n  api: Certificate Manager - SaaS ACMEv2 server\n  description: ACME clients authenticate to the Certificate Manager - SaaS ACMEv2 server with\n    External Account Binding (EAB) per RFC 8555 §7.3.4. Domain-ownership challenges (HTTP-01,\n    DNS-01, TLS-ALPN-01) are not used; issuance is governed by the configured application and\n    request policy instead.\n  docs: https://docs.venafi.cloud/vaas/configurations/acme-server-overview/\n  sources:\n  - https://docs.venafi.cloud/vaas/configurations/acme-server-overview/\n\
  mtls:\n  supported: true\n  note: POST /vedauth/authorize/certificate authenticates a client with an X.509 client\n    certificate against the self-hosted authorization server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/authentication/venafi-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Security
- Certificates
- PKI
- Machine Identity
- Identity
- Cryptography
- Key Management
- Certificate Lifecycle Management
- DevOps
- Kubernetes
- Code Signing
---
