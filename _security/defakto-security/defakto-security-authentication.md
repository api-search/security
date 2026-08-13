---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Defakto Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Defakto Security declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Defakto Security
provider_slug: defakto-security
scheme_count: 5
schemes:
- algorithm: Ed25519
  applies_to: machine
  cli: spirlctl login --service-account-key-id sak-<id> --private-key-file <path>
  credentials:
    key_id_prefix: sak-
    private_key_format: PEM
  description: A service account holds one or more Ed25519 public/private key pairs. The caller keeps the private key and uses it to sign an authentication challenge from the control plane; a session is returned in exchange. The private key is never transmitted.
  docs: https://d.defakto.security/iam/service-accounts.md
  id: service-account-key
  rotation: Multiple keys per service account are explicitly supported to enable zero-downtime rotation — deploy and verify the new key, then disable and delete the previous one.
  sdk_package: spirlsdk/auth/serviceaccount
  type: signature
- applies_to: machine
  auditing: WIF sessions are recorded in audit logs with the OIDC issuer, the matched claims, and the session ID; subsequent calls in the session carry the same session ID, so all activity traces back to the originating token exchange.
  description: A WIF Configuration binds a service account to an external OIDC identity provider and declares which JWT claims must match. A pipeline presents a short-lived platform-issued OIDC token (Terraform Cloud, GitHub Actions, GitLab, Jenkins) and receives a standard service account session with that account's role and realm assignments. No long-lived secret is stored anywhere.
  docs: https://d.defakto.security/iam/wif-issuers.md
  id: workload-identity-federation
  requires:
    wif_issuer: An organization-wide record registering the external OIDC provider and holding its key material. Created by org administrators or owners; any org member may create a WIF Configuration on a service account they own referencing an existing issuer.
  type: oidc-token-exchange
- applies_to: human
  cli_variants:
  - spirlctl login
  - spirlctl login --org <org>
  - spirlctl login --hint <email>
  - spirlctl login --headless
  - spirlctl whoami
  - spirlctl logout
  description: Browser-based OAuth login used by spirlctl and the web console. Default IdP is Google; organizations can be selected explicitly with --org. A headless device-style flow is available for SSH sessions and CI by printing a URL and accepting a pasted code.
  docs: https://d.defakto.security/cli/spirlctl/login-logout.md
  id: interactive-oauth
  sdk_package: spirlsdk/auth/oauth2
  session_storage: ~/.spirl/config.json
  type: oauth2
- applies_to: human
  description: OIDC-based single sign-on for organizations, configured per org.
  docs: https://d.defakto.security/iam/enterprise-sso.md
  id: enterprise-sso
  type: openIdConnect
- applies_to: internal
  description: The SDK ships an explicit no-auth transport (spirlsdk/auth/none.go) for unauthenticated calls. Present in the client library; not a public access path.
  id: none
  sdk_package: spirlsdk/auth/none
  type: none
slug: defakto-security-authentication
source_filename: defakto-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://d.defakto.security/iam/service-accounts.md\ndocs:\n- https://d.defakto.security/iam/service-accounts.md\n- https://d.defakto.security/iam/roles.md\n- https://d.defakto.security/iam/wif-issuers.md\n- https://d.defakto.security/iam/enterprise-sso.md\n- https://d.defakto.security/cli/spirlctl/login-logout.md\n- https://d.defakto.security/mint/configuration/token-exchange.md\nnote: >-\n  Defakto is an identity company, and its own API reflects that: there is no API key anywhere\n  in the product. Every caller — human or machine — authenticates into a short-lived session,\n  and the two machine paths are an Ed25519 challenge-signing key pair or Workload Identity\n  Federation against an external OIDC issuer, which stores no long-lived secret at all.\n  Authorization is role-based (five hierarchical org roles plus one realm-scoped role), not\n  OAuth-scope-based, so there is no scopes/ artifact for this provider — the roles\
  \ table is\n  the permission surface. Derived from the Go SDK's auth packages\n  (spirlsdk/auth/{oauth2,serviceaccount}) and the published IAM documentation.\ntransport:\n  protocol: gRPC over HTTP/2\n  tls: required\n  port: 443\n  hosts:\n  - https://api.defakto.security\n  - https://api.spirl.com\nschemes:\n- id: service-account-key\n  type: signature\n  algorithm: Ed25519\n  applies_to: machine\n  description: >-\n    A service account holds one or more Ed25519 public/private key pairs. The caller keeps\n    the private key and uses it to sign an authentication challenge from the control plane;\n    a session is returned in exchange. The private key is never transmitted.\n  credentials:\n    key_id_prefix: sak-\n    private_key_format: PEM\n  rotation: >-\n    Multiple keys per service account are explicitly supported to enable zero-downtime\n    rotation — deploy and verify the new key, then disable and delete the previous one.\n  sdk_package: spirlsdk/auth/serviceaccount\n  cli:\
  \ 'spirlctl login --service-account-key-id sak-<id> --private-key-file <path>'\n  docs: https://d.defakto.security/iam/service-accounts.md\n- id: workload-identity-federation\n  type: oidc-token-exchange\n  applies_to: machine\n  description: >-\n    A WIF Configuration binds a service account to an external OIDC identity provider and\n    declares which JWT claims must match. A pipeline presents a short-lived platform-issued\n    OIDC token (Terraform Cloud, GitHub Actions, GitLab, Jenkins) and receives a standard\n    service account session with that account's role and realm assignments. No long-lived\n    secret is stored anywhere.\n  requires:\n    wif_issuer: >-\n      An organization-wide record registering the external OIDC provider and holding its key\n      material. Created by org administrators or owners; any org member may create a WIF\n      Configuration on a service account they own referencing an existing issuer.\n  auditing: >-\n    WIF sessions are recorded in audit\
  \ logs with the OIDC issuer, the matched claims, and the\n    session ID; subsequent calls in the session carry the same session ID, so all activity\n    traces back to the originating token exchange.\n  docs: https://d.defakto.security/iam/wif-issuers.md\n- id: interactive-oauth\n  type: oauth2\n  applies_to: human\n  description: >-\n    Browser-based OAuth login used by spirlctl and the web console. Default IdP is Google;\n    organizations can be selected explicitly with --org. A headless device-style flow is\n    available for SSH sessions and CI by printing a URL and accepting a pasted code.\n  session_storage: ~/.spirl/config.json\n  sdk_package: spirlsdk/auth/oauth2\n  cli_variants:\n  - spirlctl login\n  - spirlctl login --org <org>\n  - spirlctl login --hint <email>\n  - spirlctl login --headless\n  - spirlctl whoami\n  - spirlctl logout\n  docs: https://d.defakto.security/cli/spirlctl/login-logout.md\n- id: enterprise-sso\n  type: openIdConnect\n  applies_to: human\n  description:\
  \ OIDC-based single sign-on for organizations, configured per org.\n  docs: https://d.defakto.security/iam/enterprise-sso.md\n- id: none\n  type: none\n  applies_to: internal\n  description: >-\n    The SDK ships an explicit no-auth transport (spirlsdk/auth/none.go) for unauthenticated\n    calls. Present in the client library; not a public access path.\n  sdk_package: spirlsdk/auth/none\nissued_credentials:\n  note: >-\n    Distinct from authenticating TO Defakto: these are what the platform MINTS for customer\n    workloads. They are the product, and they are what a workload subsequently presents to\n    AWS, Azure, GCP, OpenAI or Anthropic.\n  types:\n  - id: x509-svid\n    standard: SPIFFE X.509-SVID\n    description: X.509 certificate bound to a SPIFFE ID; used for mTLS between workloads.\n  - id: jwt-svid\n    standard: SPIFFE JWT-SVID\n    description: >-\n      Signed JWT bound to a SPIFFE ID with a configurable audience; the credential exchanged\n      for AWS/Azure/GCP/OpenAI/Anthropic\
  \ access via workload identity federation.\n  - id: wit-svid\n    standard: Workload Identity Token (WIT)\n    description: >-\n      Proof-of-possession bound workload token. Requires its own signing key to be enabled\n      and provisioned before use.\n    docs: https://d.defakto.security/mint/configuration/svid-issuance/wit-svid.md\ntoken_exchange:\n  endpoint: /oauth/token\n  served_by: Trust Domain Server (customer-deployed; no single public host)\n  description: >-\n    Exchanges a credential a workload already holds for a different one. Two documented\n    flows: delegation (exchange a user's token for a delegated JWT-SVID) and OAuth access\n    tokens (exchange a JWT-SVID for an OAuth access token). The OAuth issuer is configurable\n    per trust domain via --oauth-issuer / --builtin-oauth-issuer as of spirlctl 0.35.0.\n  docs: https://d.defakto.security/mint/configuration/token-exchange.md\nauthorization:\n  model: rbac\n  scope_model: none\n  note: >-\n    No OAuth scopes. Permissions\
  \ are attached to hierarchical roles, each inheriting the\n    previous. A realm-scoped role layers on top of an organization role.\n  org_roles:\n  - name: Auditor\n    rank: 1\n    summary: Read-only across users, trust domains, clusters, realms, federation, config.\n  - name: Operator\n    rank: 2\n    summary: Auditor plus create/modify clusters, cluster versions, CI/CD profiles, refresh federation links, update cluster config.\n  - name: Manager\n    rank: 3\n    summary: Operator plus trust domain key lifecycle and deployment key set management.\n  - name: Administrator\n    rank: 4\n    summary: Manager plus trust domain create/register/update/delete, realm lifecycle, role assignment, WIF issuer lifecycle, developer identity policy, org/trust-domain config.\n  - name: Owner\n    rank: 5\n    summary: Administrator plus user invitation, role change and user deletion.\n  realm_roles:\n  - name: Realm Admin\n    scope: realm\n    summary: >-\n      Delegated cluster CRUD and cluster-version\
  \ registration within assigned realms only.\n      Cannot reach other realms, create or delete realms, modify realm role assignments, or\n      elevate its own privileges. Always layered on an existing org role.\n  constraints:\n  - Service accounts cannot hold the Owner role.\n  - Users can only create service accounts with a role equal to or lower than their own.\n  - Service accounts cannot create service accounts.\n  - Non-admin roles can update or delete only service accounts they created.\n  docs: https://d.defakto.security/iam/roles.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defakto-security/refs/heads/main/authentication/defakto-security-authentication.yml
summary_line: 5 schemes
tags:
- Security
- Identity
- Non-Human Identity
- Workload Identity
- SPIFFE
- Authentication
- Zero Trust
- Secrets Management
- Kubernetes
- CI/CD
- Cloud Security
- gRPC
- Machine Identity
- Agentic AI
---
