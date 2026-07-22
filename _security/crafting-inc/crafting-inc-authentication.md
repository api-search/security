---
api_key_in: []
auth_types:
- token
- sso
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Crafting Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crafting, Inc. secures its APIs with token, sso, and mutualTLS across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crafting, Inc.
provider_slug: crafting-inc
scheme_count: 5
schemes:
- description: Interactive user authentication against the org deployment via the CLI (`cs login`) after `cs config set server_url https://SYS-DOMAIN`.
  name: UserLogin
  scheme: cs login
  sources:
  - https://docs.sandboxes.cloud/guides/developers/onboard-guide.html
  type: interactive
- description: Organizations connect their own IdP via identity federation for user sign-in.
  name: IdentityFederation
  sources:
  - https://docs.sandboxes.cloud/guides/admin/setup-identity-federation.html
  type: sso
- description: Machine identities (service accounts) authenticate with a LoginToken that is minted after the service account is created; an optional expiry can be set. Used as `cs login -t LOGIN-TOKEN` or the web URL https://SYS-DOMAIN/auth/token/LOGIN-TOKEN.
  in: token
  name: ServiceAccountLoginToken
  sources:
  - https://docs.sandboxes.cloud/concepts/service-account.html
  type: token
- description: Service accounts also carry an SSH keypair usable as a VCS deploy key; public key via `cs secret show --owner=SERVICE_ACCOUNT_EMAIL default-ssh-0`.
  name: ServiceAccountSSHKey
  sources:
  - https://docs.sandboxes.cloud/concepts/service-account.html
  type: ssh-keypair
- description: Internal workload-to-workload communication uses mTLS with certificates mutually verified by both parties; external traffic is HTTPS/TLS 1.2+.
  name: WorkloadMTLS
  sources:
  - https://docs.sandboxes.cloud/security.html
  type: mutualTLS
slug: crafting-inc-authentication
source_filename: crafting-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.sandboxes.cloud/concepts/service-account.html\ndocs: https://docs.sandboxes.cloud/security.html\nnote: >-\n  Crafting does not publish a REST OpenAPI, so this profile is derived from the\n  documented access model rather than from securitySchemes. Access is via the\n  `cs` CLI / Web Console against an organization deployment (server_url).\nsummary:\n  types: [token, sso, mutualTLS]\n  human_identity: SSO / identity federation (org users)\n  machine_identity: service accounts with LoginToken + SSH deploy keys\nschemes:\n  - name: UserLogin\n    type: interactive\n    scheme: cs login\n    description: >-\n      Interactive user authentication against the org deployment via the CLI\n      (`cs login`) after `cs config set server_url https://SYS-DOMAIN`.\n    sources: [https://docs.sandboxes.cloud/guides/developers/onboard-guide.html]\n  - name: IdentityFederation\n    type: sso\n    description: >-\n      Organizations\
  \ connect their own IdP via identity federation for user\n      sign-in.\n    sources: [https://docs.sandboxes.cloud/guides/admin/setup-identity-federation.html]\n  - name: ServiceAccountLoginToken\n    type: token\n    in: token\n    description: >-\n      Machine identities (service accounts) authenticate with a LoginToken that\n      is minted after the service account is created; an optional expiry can be\n      set. Used as `cs login -t LOGIN-TOKEN` or the web URL\n      https://SYS-DOMAIN/auth/token/LOGIN-TOKEN.\n    sources: [https://docs.sandboxes.cloud/concepts/service-account.html]\n  - name: ServiceAccountSSHKey\n    type: ssh-keypair\n    description: >-\n      Service accounts also carry an SSH keypair usable as a VCS deploy key;\n      public key via `cs secret show --owner=SERVICE_ACCOUNT_EMAIL default-ssh-0`.\n    sources: [https://docs.sandboxes.cloud/concepts/service-account.html]\n  - name: WorkloadMTLS\n    type: mutualTLS\n    description: >-\n      Internal workload-to-workload\
  \ communication uses mTLS with certificates\n      mutually verified by both parties; external traffic is HTTPS/TLS 1.2+.\n    sources: [https://docs.sandboxes.cloud/security.html]\nroles:\n  - Admin\n  - Member\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crafting-inc/refs/heads/main/authentication/crafting-inc-authentication.yml
summary_line: token/sso/mutualTLS · 5 schemes
tags:
- Company
- Developer Tools
- AI Sandboxes
- Coding Agents
- Developer Environments
- CI/CD
- Kubernetes
- Developer Productivity
- Infrastructure
---
