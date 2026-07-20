---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Avify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Avify
provider_slug: avify
scheme_count: 1
schemes:
- applies_to:
  - https://api.avify.com/graphql
  - https://api.avify.com/api/v1
  credential_management: https://app.avify.com/dashboard/settings/integrations-new
  in: header
  name: ApiKeyAuth
  parameter_name: api-key
  sources:
  - https://avify.com/docs/autenticacion-api
  type: apiKey
slug: avify-authentication
source_filename: avify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://avify.com/docs/autenticacion-api\ndocs: https://avify.com/docs/autenticacion-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_names: [api-key]\n  oauth2_flows: []\n  note: >-\n    Avify authenticates every request (GraphQL and REST) with a single API key\n    sent in the api-key header. Bearer tokens are explicitly NOT used. Tokens are\n    generated in the dashboard at app.avify.com under Configuración > Integraciones\n    > API. A token grants full privileges on the account and may be set to expire\n    or never expire; the dashboard displays the token value only once at creation.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: api-key\n    applies_to: [https://api.avify.com/graphql, https://api.avify.com/api/v1]\n    credential_management: https://app.avify.com/dashboard/settings/integrations-new\n    sources: [https://avify.com/docs/autenticacion-api]\ntest:\n\
  \  operation: 'GET https://api.avify.com/api/v1/test  (or GraphQL query { apiTest })'\n  success_example: '{\"ok\":\"ok\"}'\n  auth_failure_example: '{\"error\":{\"code\":\"A-34\",\"displayMessage\":\"Usuario no autenticado\",\"lang\":\"es\"},\"status\":401}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avify/refs/heads/main/authentication/avify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Commerce
- eCommerce
- CRM
- WhatsApp
- Conversational Commerce
- Inventory
- Point of Sale
- Payments
- Orders
- GraphQL
- Latin America
- SMB
---
