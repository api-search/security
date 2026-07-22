---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Yieldxyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yield.xyz secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yield.xyz
provider_slug: yieldxyz
scheme_count: 1
schemes:
- description: 'API keys are created within a Project on the Yield.xyz Dashboard. The key value

    is passed as the X-API-KEY header on every request (and used when integrating the

    Widget). A 401 is returned on unauthenticated requests.

    '
  in: header
  name: apiKey
  parameter_name: X-API-KEY
  sources:
  - https://docs.yield.xyz/docs/creating-an-api-key
  type: apiKey
slug: yieldxyz-authentication
source_filename: yieldxyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.yield.xyz/docs/creating-an-api-key\ndocs: https://docs.yield.xyz/docs/creating-an-api-key\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  description: |\n    API keys are created within a Project on the Yield.xyz Dashboard. The key value\n    is passed as the X-API-KEY header on every request (and used when integrating the\n    Widget). A 401 is returned on unauthenticated requests.\n  sources: [https://docs.yield.xyz/docs/creating-an-api-key]\ndashboard_access:\n  rbac: https://docs.yield.xyz/docs/rbac\n  sso: https://docs.yield.xyz/docs/yieldxyz-sso-setup-guide\n  roles: [Owner, Admin, Operator, Member]\n  sso_protocols: [SAML, OIDC]\nprogrammatic_access:\n  docs: https://docs.yield.xyz/docs/programmatic-access\n  description: |\n    A Programmatic API automates project provisioning, API key creation, yield\n    enablement,\
  \ fees, and reporting.\nnotes: |\n  Key auth only — no OAuth2 scope surface is documented, so scopes/ is intentionally\n  omitted. Dashboard access (distinct from API auth) supports RBAC roles and SAML/OIDC SSO.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yieldxyz/refs/heads/main/authentication/yieldxyz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto Web3
- Staking
- DeFi
- Yield
- Blockchain
- Restaking
- Vaults
- Web3 Infrastructure
- Non-Custodial
---
