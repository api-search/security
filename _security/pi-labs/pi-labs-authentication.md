---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pi Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pi Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pi Labs
provider_slug: pi-labs
scheme_count: 1
schemes:
- env_var: WITHPI_API_KEY
  in: header
  key_name: Authorization
  name: apiKey
  scheme: bearer
  sources:
  - https://code.withpi.ai/quickstart
  type: apiKey
slug: pi-labs-authentication
source_filename: pi-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://code.withpi.ai/quickstart\ndocs: https://code.withpi.ai/quickstart\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >-\n  Pi Labs (Pi Client) authenticates every REST request with a single API key.\n  The official SDKs read the key from the WITHPI_API_KEY environment variable\n  (e.g. PiClient(api_key=os.environ[\"WITHPI_API_KEY\"])) and send it as a bearer\n  token on the Authorization header. A free API key is issued from the Pi Labs\n  account page. No OAuth2 / OpenID Connect / scope surface is documented, so\n  there is no scopes/ artifact for this provider.\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    key_name: Authorization\n    scheme: bearer\n    env_var: WITHPI_API_KEY\n    sources: [https://code.withpi.ai/quickstart]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pi-labs/refs/heads/main/authentication/pi-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI
- Evaluation
- LLM
- Scoring
- Machine Learning
- Developer Tools
---
