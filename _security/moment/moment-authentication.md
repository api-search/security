---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Moment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moment secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moment
provider_slug: moment
scheme_count: 1
schemes:
- detail: Requests authenticate with a Moment-issued API key. The caller's organization is resolved server-side from the authenticated API key (e.g. document uploads and organization-scoped reads/writes are keyed to the org that owns the API key). Exact header name is not published in the public docs index.
  environments:
  - detail: Production API keys operate against live venues and dealers.
    name: production
  - detail: Separate "Prod Paper" (UAT) API keys route to Moment's Simulation engine sandbox with no real financial impact.
    name: prod-paper-uat
  in: header
  name: MomentApiKey
  type: apiKey
slug: moment-authentication
source_filename: moment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource:\n  - https://docs.moment.com/reference/getting-started-with-your-api\n  - https://docs.moment.com/reference/uat-testing-environment\n  - llms/moment-llms.txt\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: MomentApiKey\n    type: apiKey\n    in: header\n    detail: >-\n      Requests authenticate with a Moment-issued API key. The caller's\n      organization is resolved server-side from the authenticated API key\n      (e.g. document uploads and organization-scoped reads/writes are keyed to\n      the org that owns the API key). Exact header name is not published in the\n      public docs index.\n    environments:\n      - name: production\n        detail: Production API keys operate against live venues and dealers.\n      - name: prod-paper-uat\n        detail: >-\n          Separate \"Prod Paper\" (UAT) API keys route to Moment's Simulation\n          engine sandbox with no real\
  \ financial impact.\nnetwork_controls:\n  fix_ip_allowlist: >-\n    Organizations connecting over FIX manage an IP allowlist via the API\n    (getfixipallowlist / addfixipallowlist / removefixipallowlist) plus a\n    general organization IP allowlist (updateorganizationipallowlist).\nnotes: >-\n  No OpenAPI was published at a discoverable URL, so securityScheme details were\n  captured from the docs rather than derived. OAuth2 is not used; this is a\n  key-auth provider, so scopes/ is intentionally omitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moment/refs/heads/main/authentication/moment-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fixed Income
- Bonds
- Trading
- Market Data
- Reference Data
- Investment Management
- Wealth Management
- Brokerage
- Financial Services
- Fintech
---
