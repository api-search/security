---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Attackiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: AttackIQ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AttackIQ
provider_slug: attackiq
scheme_count: 1
schemes:
- description: 'The AttackIQ Platform authenticates API requests with a per-user API token passed in the Authorization request header using the Django REST Framework "Token" scheme (Authorization: Token <token>). Tokens are minted in the console under Administration -> API Keys with a chosen expiration; an expired token is revoked and regenerated there. The token inherits the permissions of the user account it belongs to.'
  header: Authorization
  in: header
  name: PlatformToken
  scheme_prefix: Token
  sources:
  - https://help.attackiq.com/hc/en-us/categories/api
  - https://pypi.org/project/aiq-platform-api/
  - https://docs.swimlane.com/connectors/attackiq
  token_management:
    expiration: user-selectable
    generate: Administration -> API Keys -> Generate
    revoke: supported
  type: apiKey
slug: attackiq-authentication
source_filename: attackiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.attackiq.com/hc/en-us/categories/api\ndocs: https://help.attackiq.com/hc/en-us/categories/api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: PlatformToken\n    type: apiKey\n    in: header\n    header: Authorization\n    scheme_prefix: Token\n    description: >-\n      The AttackIQ Platform authenticates API requests with a per-user API token\n      passed in the Authorization request header using the Django REST Framework\n      \"Token\" scheme (Authorization: Token <token>). Tokens are minted in the\n      console under Administration -> API Keys with a chosen expiration; an\n      expired token is revoked and regenerated there. The token inherits the\n      permissions of the user account it belongs to.\n    token_management:\n      generate: Administration -> API Keys -> Generate\n      expiration: user-selectable\n      revoke: supported\n    sources:\n     \
  \ - https://help.attackiq.com/hc/en-us/categories/api\n      - https://pypi.org/project/aiq-platform-api/\n      - https://docs.swimlane.com/connectors/attackiq\nnotes: >-\n  No OpenAPI/securitySchemes are published, so this profile was searched from the\n  provider help center and the official aiq-platform-api SDK (which sends the\n  token via the ATTACKIQ_PLATFORM_API_TOKEN env var). The platform is not an\n  OAuth2/OIDC provider; there is no scope surface (token = full user permissions),\n  so no scopes/ artifact is emitted. On-prem deployments may present self-signed\n  certificates; the SDK/CLI expose insecure / custom-CA options for that case.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attackiq/refs/heads/main/authentication/attackiq-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Breach and Attack Simulation
- Continuous Threat Exposure Management
- Security Validation
- MITRE ATT&CK
- Threat Exposure Management
---
