---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Delhivery Authentication
name_suffix: Authentication
oauth_flows: []
overview: Delhivery secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Delhivery
provider_slug: delhivery
scheme_count: 1
schemes:
- description: Client API token issued from the Delhivery One developer portal (ucp.delhivery.com / one.delhivery.com developer-portal). Sent on every request in the Authorization header as `Token <api_token>`. Test-environment and production-environment tokens differ.
  format: Token <api_token>
  header: Authorization
  in: header
  name: ClientToken
  sources:
  - https://delhivery-express-api-doc.readme.io/reference/must-to-have-for-integration
  type: apiKey
slug: delhivery-authentication
source_filename: delhivery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://delhivery-express-api-doc.readme.io/reference/introduction-1\ndocs: https://help.delhivery.com/docs/client-developer-portal-1\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Delhivery APIs authenticate with a per-client API token issued from the Delhivery\n    One developer portal. The token is passed in the request headers. There is no\n    public OAuth 2.0 / OpenID Connect flow documented for the Express and B2C APIs;\n    scopes therefore do not apply. Testing and production use distinct base URLs and,\n    typically, distinct tokens.\nschemes:\n- name: ClientToken\n  type: apiKey\n  in: header\n  header: Authorization\n  format: 'Token <api_token>'\n  description: >-\n    Client API token issued from the Delhivery One developer portal\n    (ucp.delhivery.com / one.delhivery.com developer-portal). Sent on every request\n    in the Authorization header as `Token <api_token>`.\
  \ Test-environment and\n    production-environment tokens differ.\n  sources:\n  - https://delhivery-express-api-doc.readme.io/reference/must-to-have-for-integration\nenvironments:\n- name: staging\n  base_url: https://staging-express.delhivery.com\n- name: production\n  base_url: https://track.delhivery.com\ncredentials:\n  issuance: Delhivery One developer portal (login required)\n  docs: https://one.delhivery.com/developer-portal/documents\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delhivery/refs/heads/main/authentication/delhivery-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Logistics
- Shipping
- Supply Chain
- Freight
- Ecommerce
- Tracking
- Fulfillment
- India
---
