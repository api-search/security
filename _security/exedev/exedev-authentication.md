---
api_key_in:
- header
auth_types:
- ssh-key
- http-bearer
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Exedev Authentication
name_suffix: Authentication
oauth_flows: []
overview: exe.dev secures its APIs with ssh-key, http-bearer, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: exe.dev
provider_slug: exedev
scheme_count: 3
schemes:
- description: Primary auth for VM management. Your SSH public key identifies your exe.dev account. `ssh exe.dev <command>` (the lobby REPL) and `ssh <vm>.exe.xyz` (direct VM shell) both authenticate with your registered SSH key.
  docs: https://exe.dev/docs/cli-ssh-key.md
  name: ssh-public-key
  scheme: publickey
  type: ssh
- bearerFormat: exe1 signed token
  constraints:
    max_token_size: 8KB
    timestamp_range: 2000-01-01 to 2100-01-01
  default_allowed_cmds:
  - help
  - ls
  - new
  - whoami
  - ssh-key list
  - share show
  - exe0-to-exe1
  - team
  - team members
  description: Bearer token for the HTTPS API (POST https://exe.dev/exec). Tokens are prefixed `exe1.` and are signed JSON carrying exp/nbf/cmds/ctx claims. Generated with `ssh exe.dev ssh-key generate-api-key --exp=30d`, or created locally by signing with your SSH key.
  docs: https://exe.dev/docs/https-api-local-key.md
  header: 'Authorization: Bearer [example key]'
  name: https-api-bearer
  scheme: bearer
  token_claims:
    cmds: allow-list of permitted commands (subcommands must be listed explicitly)
    ctx: custom JSON context data
    exp: Unix expiry timestamp (strongly recommended)
    nbf: Unix not-before timestamp
  type: http
- description: exe.dev exposes an OIDC discovery document (issuer https://exe.dev, RS256, id_token response type, jwks at https://exe.dev/.oidc/jwks.json). Team SSO can federate via Google OAuth or OIDC.
  docs: https://exe.dev/docs/teams/sso.md
  name: openid-connect
  openIdConnectUrl: https://exe.dev/.well-known/openid-configuration
  type: openIdConnect
slug: exedev-authentication
source_filename: exedev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://exe.dev/docs/https-api.md\ndocs: https://exe.dev/docs/https-api.md\nsummary:\n  types: [ssh-key, http-bearer, openIdConnect]\n  api_key_in: [header]\n  primary: SSH public-key authentication\nschemes:\n- name: ssh-public-key\n  type: ssh\n  scheme: publickey\n  description: >-\n    Primary auth for VM management. Your SSH public key identifies your exe.dev\n    account. `ssh exe.dev <command>` (the lobby REPL) and `ssh <vm>.exe.xyz` (direct\n    VM shell) both authenticate with your registered SSH key.\n  docs: https://exe.dev/docs/cli-ssh-key.md\n- name: https-api-bearer\n  type: http\n  scheme: bearer\n  bearerFormat: exe1 signed token\n  description: >-\n    Bearer token for the HTTPS API (POST https://exe.dev/exec). Tokens are prefixed\n    `exe1.` and are signed JSON carrying exp/nbf/cmds/ctx claims. Generated with\n    `ssh exe.dev ssh-key generate-api-key --exp=30d`, or created locally by signing\n    with your\
  \ SSH key.\n  header: 'Authorization: Bearer [example key]'\n  token_claims:\n    exp: Unix expiry timestamp (strongly recommended)\n    nbf: Unix not-before timestamp\n    cmds: allow-list of permitted commands (subcommands must be listed explicitly)\n    ctx: custom JSON context data\n  default_allowed_cmds: [help, ls, new, whoami, \"ssh-key list\", \"share show\", exe0-to-exe1, team, \"team members\"]\n  constraints:\n    max_token_size: 8KB\n    timestamp_range: 2000-01-01 to 2100-01-01\n  docs: https://exe.dev/docs/https-api-local-key.md\n- name: openid-connect\n  type: openIdConnect\n  openIdConnectUrl: https://exe.dev/.well-known/openid-configuration\n  description: >-\n    exe.dev exposes an OIDC discovery document (issuer https://exe.dev, RS256,\n    id_token response type, jwks at https://exe.dev/.oidc/jwks.json). Team SSO can\n    federate via Google OAuth or OIDC.\n  docs: https://exe.dev/docs/teams/sso.md\nnotes: >-\n  \"Login with exe\" is a separate proxy-layer auth for\
  \ apps hosted on exe.dev VMs — it\n  injects X-ExeDev-UserID and X-ExeDev-Email headers into authenticated requests rather\n  than issuing OAuth tokens (see https://exe.dev/docs/login-with-exe.md).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exedev/refs/heads/main/authentication/exedev-authentication.yml
summary_line: ssh-key/http-bearer/openIdConnect · 3 schemes
tags:
- Company
- Developer Tools
- Cloud Computing
- Virtual Machines
- Sandbox
- AI Agents
- Infrastructure
- SSH
---
