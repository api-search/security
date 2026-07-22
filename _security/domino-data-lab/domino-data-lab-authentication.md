---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Domino Data Lab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Domino Data Lab secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Domino Data Lab
provider_slug: domino-data-lab
scheme_count: 1
schemes:
- description: Domino Platform REST API requests authenticate with a per-user API key passed in the X-Domino-Api-Key request header. The key is obtained from the user account settings ("Get API key") of the Domino instance.
  docs: https://docs.dominodatalab.com/en/cloud/api_guide/8c929e/domino-platform-api-reference/
  in: header
  name: DominoApiKey
  parameter_name: X-Domino-Api-Key
  type: apiKey
slug: domino-data-lab-authentication
source_filename: domino-data-lab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.dominodatalab.com/en/cloud/api_guide/8c929e/domino-platform-api-reference/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: DominoApiKey\n    type: apiKey\n    in: header\n    parameter_name: X-Domino-Api-Key\n    description: >-\n      Domino Platform REST API requests authenticate with a per-user API key passed\n      in the X-Domino-Api-Key request header. The key is obtained from the user account\n      settings (\"Get API key\") of the Domino instance.\n    docs: https://docs.dominodatalab.com/en/cloud/api_guide/8c929e/domino-platform-api-reference/\nsdk_auth:\n  # python-domino resolves credentials in this order\n  order: [api_proxy, auth_token, domino_token_file, api_key]\n  env:\n    - DOMINO_API_PROXY\n    - DOMINO_TOKEN_FILE\n    - DOMINO_USER_API_KEY\n    - DOMINO_API_HOST\nnotes: >-\n  Base URL is the customer's own Domino deployment host (self-managed or\
  \ Domino Cloud);\n  there is no single shared public API host. API paths follow /api/{service}/{version}/...\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domino-data-lab/refs/heads/main/authentication/domino-data-lab-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- MLOps
- Data Science
- Machine Learning
- AI Platform
- Model Monitoring
- Enterprise AI
---
