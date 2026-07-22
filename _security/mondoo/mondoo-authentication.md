---
api_key_in: []
auth_types:
- bearer-token
- oidc
description: ''
kind: authentication
layout: security
method: searched
name: Mondoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mondoo secures its APIs with bearer-token and oidc across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mondoo
provider_slug: mondoo
scheme_count: 2
schemes:
- description: Programmatic access to the Mondoo Platform GraphQL API uses service account API tokens. Service accounts are created at space or organization scope and carry a role. Credentials are issued as JSON (or base64-encoded JSON) and supplied to cnspec/cnquery via --config or MONDOO_CONFIG_PATH, and to the Go SDK via option.WithAPIToken.
  name: ServiceAccountToken
  scheme: bearer
  sources:
  - https://mondoo.com/docs/platform/maintain/access/service_accounts/
  type: http
- description: Each region runs a Security Token Service exposing OIDC discovery at /.well-known/openid-configuration (issuers https://sts.us.mondoo.com and https://sts.eu.mondoo.com). RS256-signed id tokens, scope "openid".
  name: OIDC-STS
  openid_configuration:
  - https://us.api.mondoo.com/.well-known/openid-configuration
  - https://eu.api.mondoo.com/.well-known/openid-configuration
  type: openIdConnect
slug: mondoo-authentication
source_filename: mondoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mondoo.com/docs/platform/maintain/access/service_accounts/\ndocs: https://mondoo.com/docs/platform/maintain/access/service_accounts/\nsummary:\n  types:\n  - bearer-token\n  - oidc\n  token_model: service-account-api-token\n  regions:\n  - us\n  - eu\nschemes:\n- name: ServiceAccountToken\n  type: http\n  scheme: bearer\n  description: >-\n    Programmatic access to the Mondoo Platform GraphQL API uses service account\n    API tokens. Service accounts are created at space or organization scope and\n    carry a role. Credentials are issued as JSON (or base64-encoded JSON) and\n    supplied to cnspec/cnquery via --config or MONDOO_CONFIG_PATH, and to the Go\n    SDK via option.WithAPIToken.\n  sources:\n  - https://mondoo.com/docs/platform/maintain/access/service_accounts/\n- name: OIDC-STS\n  type: openIdConnect\n  description: >-\n    Each region runs a Security Token Service exposing OIDC discovery at\n    /.well-known/openid-configuration\
  \ (issuers https://sts.us.mondoo.com and\n    https://sts.eu.mondoo.com). RS256-signed id tokens, scope \"openid\".\n  openid_configuration:\n  - https://us.api.mondoo.com/.well-known/openid-configuration\n  - https://eu.api.mondoo.com/.well-known/openid-configuration\nroles:\n- name: Viewer\n  description: Read-only browsing.\n- name: Editor\n  description: Make modifications except deleting the space.\n- name: Owner\n  description: Make all changes except reporting scan results.\n- name: Agent\n  description: Execute policies and report scan results.\nscopes_of_access:\n- space\n- organization\nendpoints:\n  us: https://us.api.mondoo.com/query\n  eu: https://eu.api.mondoo.com/query\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mondoo/refs/heads/main/authentication/mondoo-authentication.yml
summary_line: bearer-token/oidc · 2 schemes
tags:
- Company
- Cybersecurity
- Security
- Vulnerability Management
- Compliance
- Cloud Security
- Policy as Code
- DevSecOps
- GraphQL
- SAST
---
