---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Carapace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carapace declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Carapace
provider_slug: carapace-bot
scheme_count: 4
schemes:
- description: Agents call POST /v1/request on the enclave with the header Authorization Bearer cpk_... over attested TLS. The owner's CLI mints the key as cpk_<fingerprint>_<random> and signs a grant for it; the server stores only a lookup hash and the grant. Grants default to a 30-day TTL (--ttl-days).
  name: agentApiKey
  scheme: bearer
  source: https://github.com/99darwin/carapace-oss/blob/main/enclave/src/carapace_enclave/server.py
  surface: enclave (https://<enclave ip>:8443)
  type: http
- bearerFormat: JWT
  description: Account login by password or passkey (WebAuthn, user verification required) returns access JWTs carrying jti, iss and aud; refresh tokens are single use and rotated, and reuse of a rotated token revokes the whole family. Logout blacklists the jti.
  name: userJwt
  scheme: bearer
  source: https://github.com/99darwin/carapace-oss/blob/main/server/README.md
  surface: control-plane server (/v1/*)
  type: http
- description: Enclaves authenticate to the server with a Confidential Space OIDC token whose audience is CARAPACE_PUBLIC_URL; Google's signing keys are found by OIDC discovery. Receipt uploads are additionally signed with X-Carapace-Timestamp (unix seconds, +/-60 s) and X-Carapace-Signature (base64 Ed25519 over the message with the per-boot receipt key).
  name: enclaveOidc
  source: https://github.com/99darwin/carapace-oss/blob/main/server/README.md
  surface: control-plane server (/internal/*)
  type: openIdConnect
- description: Every object the enclave trusts (secret envelopes, policies, API-key grants) is signed with the owner's Ed25519 owner key, whose seed never leaves the owner's device.
  name: ownerKeySignature
  source: https://github.com/99darwin/carapace-oss/blob/main/docs/design/owner-signing.md
  type: signature
slug: carapace-bot-authentication
source_filename: carapace-bot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://github.com/99darwin/carapace-oss/blob/main/server/README.md\ndocs: https://github.com/99darwin/carapace-oss/blob/main/docs/ARCHITECTURE.md\nnote: No OpenAPI is published (the server exposes /openapi.json only in dev mode), so this profile is read from the project docs and source docstrings, not derived from a contract. Every deployment is self-hosted in the user's own GCP project.\nschemes:\n- name: agentApiKey\n  type: http\n  scheme: bearer\n  surface: enclave (https://<enclave ip>:8443)\n  description: Agents call POST /v1/request on the enclave with the header Authorization Bearer cpk_... over attested TLS. The owner's CLI mints the key as cpk_<fingerprint>_<random> and signs a grant for it; the server stores only a lookup hash and the grant. Grants default to a 30-day TTL (--ttl-days).\n  source: https://github.com/99darwin/carapace-oss/blob/main/enclave/src/carapace_enclave/server.py\n- name: userJwt\n  type:\
  \ http\n  scheme: bearer\n  bearerFormat: JWT\n  surface: control-plane server (/v1/*)\n  description: Account login by password or passkey (WebAuthn, user verification required) returns access JWTs carrying jti, iss and aud; refresh tokens are single use and rotated, and reuse of a rotated token revokes the whole family. Logout blacklists the jti.\n  source: https://github.com/99darwin/carapace-oss/blob/main/server/README.md\n- name: enclaveOidc\n  type: openIdConnect\n  surface: control-plane server (/internal/*)\n  description: Enclaves authenticate to the server with a Confidential Space OIDC token whose audience is CARAPACE_PUBLIC_URL; Google's signing keys are found by OIDC discovery. Receipt uploads are additionally signed with X-Carapace-Timestamp (unix seconds, +/-60 s) and X-Carapace-Signature (base64 Ed25519 over the message with the per-boot receipt key).\n  source: https://github.com/99darwin/carapace-oss/blob/main/server/README.md\n- name: ownerKeySignature\n  type: signature\n\
  \  description: Every object the enclave trusts (secret envelopes, policies, API-key grants) is signed with the owner's Ed25519 owner key, whose seed never leaves the owner's device.\n  source: https://github.com/99darwin/carapace-oss/blob/main/docs/design/owner-signing.md\n"
source_yaml_url: https://artifacts.apis.io/carapace-bot/authentication/carapace-bot-authentication.yml
summary_line: 4 schemes
tags:
- Company
- AI Agents
- Secrets Management
- Confidential Computing
- Security
- Open Source
- Google Cloud
- Self-Hosted
---
