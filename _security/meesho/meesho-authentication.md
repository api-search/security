---
api_key_in:
- header
api_specs:
- filename: meesho
  format: yaml
  label: Meesho Supplier / Order-Management API
  slug: meesho-supplier-order-management-api
  spec_type: Postman
  url: https://www.postman.com/meesho
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Meesho Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meesho secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Meesho
provider_slug: meesho
scheme_count: 1
schemes:
- credentials:
  - client-id
  - secret-key
  description: Per-request credential + signature headers supplied by Meesho to onboarded suppliers/partners. Reported headers include client/merchant identifier, a security/secret value, a request timestamp, and a supplier_identifier.
  headers:
  - merchant
  - security
  - timestamp
  - supplier_identifier
  in: header
  name: MeeshoSignedHeaders
  onboarding: Credentials requested from Meesho during partner onboarding (integration contact meesholink-integration@meesho.com per channel docs).
  type: apiKey
slug: meesho-authentication
source_filename: meesho-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://documentation.fynd.com/konnect/channels/marketplaces-webstores/meesho\ndocs: https://www.postman.com/meesho\nnote: >-\n  Meesho's Supplier / Order-Management API is a partner-gated integration. There\n  is no public self-service OpenAPI; credentials (client-id, secret-key) are\n  issued by Meesho during supplier/partner onboarding. Authentication is\n  performed with per-request signed headers rather than OAuth. Details below are\n  captured from the published Meesho partner integration and third-party channel\n  documentation, not from a first-party OpenAPI securityScheme.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: MeeshoSignedHeaders\n  type: apiKey\n  in: header\n  description: >-\n    Per-request credential + signature headers supplied by Meesho to onboarded\n    suppliers/partners. Reported headers include client/merchant identifier, a\n    security/secret\
  \ value, a request timestamp, and a supplier_identifier.\n  headers:\n  - merchant\n  - security\n  - timestamp\n  - supplier_identifier\n  credentials:\n  - client-id\n  - secret-key\n  onboarding: >-\n    Credentials requested from Meesho during partner onboarding (integration\n    contact meesholink-integration@meesho.com per channel docs).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meesho/refs/heads/main/authentication/meesho-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketplace
- E-Commerce
- Social Commerce
- Retail
- Marketplaces
- India
- Suppliers
---
