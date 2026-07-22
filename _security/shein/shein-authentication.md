---
api_key_in: []
auth_types:
- seller-authorization
description: ''
kind: authentication
layout: security
method: searched
name: Shein Authentication
name_suffix: Authentication
oauth_flows: []
overview: SHEIN secures its APIs with seller-authorization across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SHEIN
provider_slug: shein
scheme_count: 0
schemes: []
slug: shein-authentication
source_filename: shein-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://open.sheincorp.com/en\ndocs: https://open.sheincorp.com/\nsummary:\n  types:\n  - seller-authorization\n  note: >-\n    No public OpenAPI/Swagger securitySchemes are available to derive from — the\n    API reference is gated behind an approved Open Platform account. The auth\n    model below is captured from the public Open Platform overview.\nmodel:\n  style: seller-authorization-grant\n  description: >-\n    Integration is authorization-based. A partner applies for a SHEIN Open\n    Platform account, creates an Application, passes an application review, then\n    completes an \"Authorization Integration\" step in which the seller authorizes\n    the application (governed by the Seller Authorization Agreement) before the\n    API solutions can be called.\n  onboarding_steps:\n  - Open Platform Account Application\n  - Create Application\n  - Application Review\n  - Authorization Integration (seller authorizes the application)\n\
  \  - Solution Integration\n  api_host: https://openapi.sheincorp.com\n  unauthenticated_response: HTTP 401 application/json (requests must be authenticated and seller-authorized)\n  seller_authorization_agreement: https://open.sheincorp.com/contract?type=seller\ncontact: openapi@shein.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shein/refs/heads/main/authentication/shein-authentication.yml
summary_line: seller-authorization · 0 schemes
tags:
- Company
- Consumer
- E-commerce
- Retail
- Fashion
- Marketplace
- Fulfillment
- Logistics
- Open Platform
- Sellers
---
