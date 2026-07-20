---
api_key_in:
- query
auth_types:
- apiKey
description: The Desmos API authenticates with a single API key supplied as a URL query parameter on the calculator.js script include. There is no OAuth, no bearer token, and no server-side credential exchange — the key gates which calculator products load client-side. Production keys are issued at desmos.com/my-api; a public demo key ships in the documentation for development (see sandbox/desmos-sandbox.yml).
kind: authentication
layout: security
method: searched
name: Desmos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Desmos secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Desmos
provider_slug: desmos
scheme_count: 1
schemes:
- example: https://www.desmos.com/api/v1.12/calculator.js?apiKey=YOUR_API_KEY
  in: query
  name: apiKey
  notes: Required to load the API. The Graphing Calculator loads by default; the Four-Function, Scientific, and Geometry calculators must be separately enabled per API key. Obtain a production key at https://www.desmos.com/my-api.
  parameter: apiKey
  transport: script-url
  type: apiKey
slug: desmos-authentication
source_filename: desmos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.desmos.com/api/v1.12/docs/index.html\ndocs: https://www.desmos.com/my-api\ndescription: >-\n  The Desmos API authenticates with a single API key supplied as a URL query\n  parameter on the calculator.js script include. There is no OAuth, no bearer\n  token, and no server-side credential exchange — the key gates which calculator\n  products load client-side. Production keys are issued at desmos.com/my-api; a\n  public demo key ships in the documentation for development (see\n  sandbox/desmos-sandbox.yml).\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: query\n    parameter: apiKey\n    transport: script-url\n    example: https://www.desmos.com/api/v1.12/calculator.js?apiKey=YOUR_API_KEY\n    notes: >-\n      Required to load the API. The Graphing Calculator loads by default; the\n      Four-Function, Scientific, and Geometry calculators\
  \ must be separately\n      enabled per API key. Obtain a production key at https://www.desmos.com/my-api.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/desmos/refs/heads/main/authentication/desmos-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Education
- Mathematics
- Graphing Calculator
- Embeddable
- JavaScript
- EdTech
- Data Visualization
---
