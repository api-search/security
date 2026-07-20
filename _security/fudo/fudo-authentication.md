---
api_key_in: []
api_specs:
- filename: fudo-openapi-original.yml
  format: yaml
  label: Fudo API
  slug: fudo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fudo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fudo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fudo
provider_slug: fudo
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer token obtained from the authentication endpoint (https://auth.fu.do/api) by exchanging apiKey + apiSecret. Sent as "Authorization: Bearer <token>".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fudo-openapi-original.yml
  type: http
slug: fudo-authentication
source_filename: fudo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fudo-openapi-original.yml\ndocs: https://dev.fu.do/api/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_exchange: true\nflow:\n  description: >-\n    Fudo uses a two-step, token-based scheme. First obtain long-lived access\n    credentials (apiKey + apiSecret) by requesting API access, then exchange\n    them for a short-lived bearer token at the authentication endpoint. Send the\n    token in the Authorization header of every API request, prefixed with\n    \"Bearer \". Tokens last 24 hours; the expiry is returned in the \"exp\" field\n    (seconds since epoch) so callers can renew before expiry. API access\n    requires the Pro plan or higher, and the actions permitted depend on the\n    role assigned to the user tied to the credentials.\n  credentials:\n    apiKey: Issued per account/user; request via soporte@fu.do or Administration > Users > \"Establecer API Secret\".\n    apiSecret: Secret paired\
  \ with the apiKey; shown once and must be saved immediately.\n  token_endpoint: https://auth.fu.do/api\n  token_method: POST\n  token_request_content_type: application/json\n  token_request_example: |-\n    curl -X POST https://auth.fu.do/api \\\n         -d '{\"apiKey\":\"123456\",\"apiSecret\":\"654321\"}' \\\n         -H \"Accept: application/json\" \\\n         -H \"Content-Type: application/json\"\n  token_response_example: '{\"token\":\"1234567890\",\"exp\":\"1645387452\"}'\n  token_ttl_hours: 24\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Bearer token obtained from the authentication endpoint (https://auth.fu.do/api)\n    by exchanging apiKey + apiSecret. Sent as \"Authorization: Bearer <token>\".\n  sources:\n  - openapi/fudo-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/authentication/fudo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Restaurant
- Point of Sale
- Hospitality
- Food and Beverage
- Payments
- Inventory
- Latin America
- SaaS
---
