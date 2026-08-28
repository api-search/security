---
api_key_in: []
api_specs:
- filename: payem-ai-discovery-openapi.json
  format: json
  label: Payem AI Discovery API
  slug: payem-ai-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/openapi/payem-ai-discovery-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Payem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Payem declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Payem
provider_slug: payem
scheme_count: 0
schemes: []
slug: payem-authentication
source_filename: payem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/payem-ai-discovery-openapi.json\napi: Payem AI Discovery API\nsummary: >-\n  The only machine-readable PayEm contract declares no security schemes and requires no\n  credentials. components.securitySchemes is absent, there is no top-level security[]\n  block, and every operation was called anonymously during this pass and returned 200.\nsecurity_schemes: []\nmodel: none\nanonymous: true\nverified:\n- url: https://api.llm-discovery-api.com/functions/v1/llm-discovery/public/business?domain=payem.co\n  status: 200\n  auth_sent: none\n- url: https://api.llm-discovery-api.com/functions/v1/llm-discovery/public/products?domain=payem.co\n  status: 200\n  auth_sent: none\nproduct_api:\n  status: not-published\n  note: >-\n    PayEm's spend-management product has no public authentication documentation. There is\n    no developer portal, no API-key page and no OAuth surface. What PayEm does document,\n    on its own security page,\
  \ is end-user authentication into the application: mandatory\n    multi-factor authentication and SAML SSO through an external identity provider such\n    as Google or Okta. That is application sign-in, not API authentication, and it is\n    recorded here so a reader does not mistake one for the other.\n  source: https://www.payem.co/legal/security-and-compliance\noauth_scopes: na\nnotes:\n- The vendor host echoes CORS access-control-allow-headers listing authorization and apikey,\n  but no operation requires either and none is documented.\n- A required `domain` query parameter (payem.co) acts as the tenant selector on the shared\n  LightSite service. It is a routing key, not a credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payem/refs/heads/main/authentication/payem-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Spend Management
- Procurement
- Accounts Payable
- Corporate Cards
- Expense Management
- Financial Operations
- Invoice Processing
- FinTech
- ERP Integration
---
