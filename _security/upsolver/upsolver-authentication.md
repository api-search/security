---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Upsolver Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upsolver secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Upsolver
provider_slug: upsolver
scheme_count: 1
schemes:
- description: Personal API token created at https://sqlake.upsolver.com/Settings/api-tokens, passed with requests to the account's API URL (e.g. the api.upsolver.com service host). Used by upsolver-sdk-python (DB API 2.0 connection) and upsolver-cli.
  name: api-token
  sources:
  - https://github.com/Upsolver/upsolver-sdk-python
  - https://github.com/Upsolver/cli
  type: apiKey
slug: upsolver-authentication
source_filename: upsolver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/Upsolver/upsolver-sdk-python\ndocs: https://docs.upsolver.com/ (redirects to https://help.qlik.com/en-US/upsolver/sqlake/)\nnote: >-\n  Upsolver publishes no OpenAPI, so this profile was captured from the\n  first-party Python SDK and CLI documentation rather than derived from a\n  spec. Programmatic access to the Upsolver (SQLake) API uses a personal API\n  token generated in the SQLake console (Settings → API Tokens) together with\n  an account-specific API URL; the SDK connects with\n  upsolver.connect(token=..., api_url=...) and the CLI uses the same token +\n  API URL pair over HTTP.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: api-token\n    type: apiKey\n    description: >-\n      Personal API token created at https://sqlake.upsolver.com/Settings/api-tokens,\n      passed with requests to the account's API URL (e.g. the api.upsolver.com\n      service\
  \ host). Used by upsolver-sdk-python (DB API 2.0 connection) and\n      upsolver-cli.\n    sources:\n      - https://github.com/Upsolver/upsolver-sdk-python\n      - https://github.com/Upsolver/cli\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upsolver/refs/heads/main/authentication/upsolver-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- Data Pipelines
- Data Lakehouse
- Streaming
- ETL
- SQL
- Apache Iceberg
---
