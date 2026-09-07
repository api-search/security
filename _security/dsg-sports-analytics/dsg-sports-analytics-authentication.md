---
anonymous_access: false
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dsg Sports Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: DSG Sports Analytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DSG Sports Analytics
provider_slug: dsg-sports-analytics
scheme_count: 2
schemes:
- description: Unique client ID issued by DSG with the account. Also appears as a path segment in the request URL (/clients/{client_name}/...).
  in: query
  name: client
  parameter: client
  required: true
  sources:
  - https://dsg-api.com/doc/soccer/get_matches/1/
  type: apiKey
- description: Client authentication key issued with the account. DSG's docs state it "should not be shared or visible in code".
  in: query
  name: authkey
  parameter: authkey
  required: true
  sources:
  - https://dsg-api.com/introduction/
  - https://dsg-api.com/doc/soccer/get_matches/1/
  type: apiKey
slug: dsg-sports-analytics-authentication
source_filename: dsg-sports-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://dsg-api.com/introduction/\ndocs: https://dsg-api.com/introduction/\nnote: >-\n  Derived from the provider's own published API reference, not from an OpenAPI document - DSG\n  publishes no machine-readable contract. The introduction page describes what it calls \"3 security\n  layers\"; the per-operation doc pages (e.g. https://dsg-api.com/doc/soccer/get_matches/1/) confirm\n  the two credential parameters are carried in the query string of every request.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - query\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  transport: https-only\nschemes:\n  - name: client\n    type: apiKey\n    in: query\n    parameter: client\n    required: true\n    description: Unique client ID issued by DSG with the account. Also appears as a path segment in\n      the request URL (/clients/{client_name}/...).\n    sources:\n      - https://dsg-api.com/doc/soccer/get_matches/1/\n\
  \  - name: authkey\n    type: apiKey\n    in: query\n    parameter: authkey\n    required: true\n    description: Client authentication key issued with the account. DSG's docs state it \"should not\n      be shared or visible in code\".\n    sources:\n      - https://dsg-api.com/introduction/\n      - https://dsg-api.com/doc/soccer/get_matches/1/\nlayers:\n  - layer: 1\n    mechanism: api-key-in-url\n    description: Every client receives an authentication key with their account which must be used in\n      the API URL.\n  - layer: 2\n    mechanism: account-password\n    description: A password protecting the API account, passed separately from the API URL, so a\n      leaked API URL alone cannot be used.\n    note: The docs describe this layer but do not publish where or how the password is transmitted on\n      an API call; it is documented as an account-level protection.\n  - layer: 3\n    mechanism: domain-allowlist\n    description: DSG allowlists access to API accounts and to their\
  \ images per domain.\ncredential_issuance:\n  self_service: false\n  registration_url: https://dsg-api.com/register/\n  registration_status: >-\n    The /register/ page resolves HTTP 200 but renders no signup form, and the \"Sign up\" button is\n    commented out of the site header. The products page states credentials are issued by the DSG\n    team (\"you will receive personalized login credentials from our team\"), so onboarding is\n    sales-mediated.\n  login_url: https://dsg-api.com/login/\n  contact: sales@datasportsgroup.com\ntransport:\n  https_required: true\n  note: The docs list \"Connection refused - most likely cause is not using HTTPS\" as a failure mode.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dsg-sports-analytics/refs/heads/main/authentication/dsg-sports-analytics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analysis
- Insights
- Sports
- Sports Data
- Live Scores
- Statistics
---
