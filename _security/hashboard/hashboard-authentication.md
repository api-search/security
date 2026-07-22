---
api_key_in:
- access-key-file
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Hashboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hashboard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hashboard
provider_slug: hashboard
scheme_count: 1
schemes:
- description: An access key downloaded via `hb token` through a web-based auth flow, stored by default at ~/.hashboard/hb_access_key.json and used by the CLI and hashquery.
  docs: https://docs.hashboard.com/docs/data-ops/quickstart
  location: file (~/.hashboard/hb_access_key.json) or HASHBOARD_ env credentials
  name: accessKey
  type: apiKey
slug: hashboard-authentication
source_filename: hashboard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.hashboard.com/docs/data-ops/quickstart\ndocs: https://docs.hashboard.com/docs/data-ops/cli\nsummary:\n  types: [apiKey]\n  api_key_in: [access-key-file]\n  note: >-\n    Hashboard is a BI-as-code product with no public REST API/OpenAPI. Programmatic\n    access is via the Hashboard CLI (hb) and the hashquery Python framework, both\n    authenticated with a downloaded access key rather than an HTTP securityScheme.\nschemes:\n  - name: accessKey\n    type: apiKey\n    description: >-\n      An access key downloaded via `hb token` through a web-based auth flow, stored\n      by default at ~/.hashboard/hb_access_key.json and used by the CLI and hashquery.\n    location: file (~/.hashboard/hb_access_key.json) or HASHBOARD_ env credentials\n    docs: https://docs.hashboard.com/docs/data-ops/quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashboard/refs/heads/main/authentication/hashboard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- B2B
- Business Intelligence
- Analytics
- Data
- BI-as-Code
- Dashboards
- Data Visualization
- Developer Tools
- CLI
---
