---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Coiled Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coiled secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coiled
provider_slug: coiled
scheme_count: 1
schemes:
- description: Coiled's REST API and Python client authenticate with a static API token. The token is sent in the HTTP Authorization header using the custom "ApiToken" scheme (not Bearer). Tokens are created at https://cloud.coiled.io/profile or via `coiled login`.
  format: 'Authorization: ApiToken $COILED_API_TOKEN'
  in: header
  name: ApiToken
  parameter_name: Authorization
  sources:
  - docs
  token_creation: https://cloud.coiled.io/profile
  type: apiKey
slug: coiled-authentication
source_filename: coiled-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.coiled.io/user_guide/rest-api.html\ndocs: https://docs.coiled.io/user_guide/setup/tokens.html\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ApiToken\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    format: \"Authorization: ApiToken $COILED_API_TOKEN\"\n    description: >-\n      Coiled's REST API and Python client authenticate with a static API token.\n      The token is sent in the HTTP Authorization header using the custom\n      \"ApiToken\" scheme (not Bearer). Tokens are created at\n      https://cloud.coiled.io/profile or via `coiled login`.\n    token_creation: https://cloud.coiled.io/profile\n    sources: [docs]\nstorage:\n  - method: cli\n    value: coiled login --token <your-token>\n  - method: env_var\n    value: DASK_COILED__TOKEN\n  - method: config_file\n    value: ~/.config/dask/coiled.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coiled/refs/heads/main/authentication/coiled-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai Ml
- Cloud Computing
- Data Science
- Dask
- Python
- Distributed Computing
- Machine Learning
- Serverless
---
