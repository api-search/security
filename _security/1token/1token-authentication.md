---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 1token-1ndex-openapi.yml
  format: yaml
  label: 1Token 1ndex Public Strategy Overview API
  slug: 1token-1ndex-public-strategy-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1token/refs/heads/main/openapi/1token-1ndex-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: 1Token Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1Token declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: 1Token
provider_slug: 1token
scheme_count: 0
schemes: []
slug: 1token-authentication
source_filename: 1token-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://1token.tech/api/1ndex/v1/README.md\nspec_source: openapi/1token-1ndex-openapi.yml\ndocs: https://1token.tech/api/1ndex/v1/README.md\nsummary:\n  types: []\n  anonymous: true\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The one public 1Token API declares no security schemes and an empty top-level `security: []`,\n    and the published documentation states this explicitly: \"No authentication is currently\n    required.\" This is a documented anonymous-access posture, not a thin or missing spec — verified\n    by an unauthenticated live GET returning HTTP 200 application/json on 2026-09-05.\nschemes: []\npublic_access:\n  anonymous: true\n  scope: >-\n    Aggregate 1ndex strategy overview only. The published contract explicitly excludes\n    customer-specific data, write operations, CAM product interfaces, and third-party APIs consumed\n    by 1Token.\n  evidence:\n  - kind: spec\n    detail: 'openapi/1token-1ndex-openapi.yml:\
  \ top-level `security: []` and operation-level `security: []`'\n  - kind: docs\n    url: https://1token.tech/api/1ndex/v1/README.md\n    detail: '\"No authentication is currently required.\"'\n  - kind: probe\n    url: https://1ndex.1token.tech/api/v1/public/strategy-overview?strategy_type=DeltaNeutral\n    http_status: 200\n    detail: unauthenticated request returned 200 application/json\ngated_surfaces:\n- name: 1Token CAM\n  auth: customer login\n  url: https://1token.tech/cam-docs\n  note: >-\n    CAM technical API documentation redirects to https://1token.tech/cam-docs-login and is\n    disallowed in robots.txt. The Trust Center describes API key management, RBAC, MFA and\n    read-only API integrations for CAM, but no CAM auth reference is public.\n- name: 1ndex application\n  auth: account login\n  url: https://1ndex.1token.tech/login\n  note: The 1ndex web app requires an account; access is requested via a Calendly link.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1token/refs/heads/main/authentication/1token-authentication.yml
summary_line: 0 schemes
tags:
- Digital Assets
- Crypto
- Portfolio Management
- Risk Management
- Fund Administration
- Reconciliation
- Fund Accounting
- Institutional Finance
- DeFi
- Market Data
- Company
---
