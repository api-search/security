---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Nominal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nominal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nominal
provider_slug: nominal
scheme_count: 1
schemes:
- description: Nominal authenticates API requests with a per-user API token (bearer token), issued under Settings -> API keys in the Nominal app. The token is attached to a user and may access one or more workspaces. Tokens are supplied as a bearer credential to the Conjure REST API at https://api.gov.nominal.io/api.
  name: NominalApiKey
  scheme: bearer
  sources:
  - docs
  type: http
slug: nominal-authentication
source_filename: nominal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nominal.io/python/quickstart\ndocs: https://docs.nominal.io/python/quickstart\nsummary:\n  types: [http]\n  scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\nbase_url: https://api.gov.nominal.io/api\nschemes:\n- name: NominalApiKey\n  type: http\n  scheme: bearer\n  description: Nominal authenticates API requests with a per-user API token (bearer\n    token), issued under Settings -> API keys in the Nominal app. The token is attached\n    to a user and may access one or more workspaces. Tokens are supplied as a bearer\n    credential to the Conjure REST API at https://api.gov.nominal.io/api.\n  sources: [docs]\nconcepts:\n- name: base_url\n  description: The URL through which the Nominal API is accessed; typically https://api.gov.nominal.io/api,\n    shown under Settings -> API keys.\n- name: workspace\n  description: A mechanism to isolate datasets; each user has one or more workspaces\n    and data\
  \ in one cannot be seen from another. A token may access multiple workspaces.\n- name: profile\n  description: A named combination of base URL, API key, and workspace stored on disk\n    at ~/.config/nominal/config.yml via the `nom` CLI (recommended over embedding\n    the key in code).\nguidance: Never share or commit the Nominal API key. Prefer the `nom` CLI profile\n  store over inlining the token in scripts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nominal/refs/heads/main/authentication/nominal-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Deep Tech
- Test and Measurement
- Hardware
- Aerospace
- Telemetry
- Observability
- Industrial Data
- Data Platform
- SDKs
---
