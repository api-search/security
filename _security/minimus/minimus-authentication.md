---
api_key_in: []
auth_types: []
description: Authentication profile for the Minimus programmatic surfaces. There is no documented public OAuth2/OIDC REST API; access is via a static bearer token used by minicli, plus an open (unauthenticated) MinimOS package repository.
kind: authentication
layout: security
method: searched
name: Minimus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Minimus declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Minimus
provider_slug: minimus
scheme_count: 2
schemes:
- evidence: 'minicli docs: "All commands require MINICLI_TOKEN to be set."'
  id: minicli-token
  in: environment-or-login
  parameter: MINICLI_TOKEN
  scope: Grants access to manage private image recipes and builds for the account.
  token_management: https://images.minimus.io/manage/token
  type: bearer-token
  usage:
  - 'export MINICLI_TOKEN={token}   # CI/CD'
  - 'echo "{token}" | minicli login  # local'
- evidence: 'Package-manager docs: "the MinimOS package repository is open to all, there is no need to pass credentials."'
  id: minimos-apk-repo
  in: none
  scope: Open MinimOS package repository packages.mini.dev/os; no credentials required.
  type: none
slug: minimus-authentication
source_filename: minimus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.minimus.io/manage/minicli\ndescription: >-\n  Authentication profile for the Minimus programmatic surfaces. There is no\n  documented public OAuth2/OIDC REST API; access is via a static bearer token\n  used by minicli, plus an open (unauthenticated) MinimOS package repository.\ndocs: https://docs.minimus.io/manage/minicli\nschemes:\n- id: minicli-token\n  type: bearer-token\n  in: environment-or-login\n  parameter: MINICLI_TOKEN\n  token_management: https://images.minimus.io/manage/token\n  usage:\n  - 'export MINICLI_TOKEN={token}   # CI/CD'\n  - 'echo \"{token}\" | minicli login  # local'\n  scope: 'Grants access to manage private image recipes and builds for the account.'\n  evidence: 'minicli docs: \"All commands require MINICLI_TOKEN to be set.\"'\n- id: minimos-apk-repo\n  type: none\n  in: none\n  scope: 'Open MinimOS package repository packages.mini.dev/os; no credentials required.'\n  evidence: 'Package-manager\
  \ docs: \"the MinimOS package repository is open to all, there is no need to pass credentials.\"'\nenterprise:\n  sso: 'Enterprise SSO and RBAC for unlimited users (Enterprise plan).'\n  evidence: 'Pricing: \"Enterprise SSO and RBAC for unlimited users.\"'\nnotes: >-\n  Container image pulls from the OCI registry use standard registry auth\n  (token/credential) where images are private; public starter images are open.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minimus/refs/heads/main/authentication/minimus-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Container Images
- Container Security
- Supply Chain Security
- DevSecOps
- Compliance
- CLI
- Hardened Images
---
