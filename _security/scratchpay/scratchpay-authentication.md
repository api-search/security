---
api_key_in: []
api_specs:
- filename: scratchpay-scratchpay-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Borrower Application API
  slug: scratchpay-borrower-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-scratchpay-1.0.0-apis-swagger.yml
- filename: scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Care Credit API
  slug: scratchpay-care-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml
- filename: scratchpay-partner-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Partner Result API
  slug: scratchpay-partner-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-partner-1.0.0-apis-swagger.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Scratchpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scratchpay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scratchpay
provider_slug: scratchpay
scheme_count: 1
schemes:
- format: Bearer <integration-token>
  header_name: Authorization
  location: header
  name: partnerBearerToken
  scheme: bearer
  sources:
  - openapi/scratchpay-scratchpay-1.0.0-apis-swagger.yml
  - openapi/scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml
  - openapi/scratchpay-partner-1.0.0-apis-swagger.yml
  token_provisioning: 'The integration token is issued to the practice/partner from the Scratch Dashboard (Account tab -> Integration Token, https://my.scratchpay.com/#/clinic/token).

    '
  type: http
slug: scratchpay-authentication
source_filename: scratchpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/scratchpay-scratchpay-1.0.0-apis-swagger.yml\ndocs: https://scratchpay-lending.stonly.com/kb/guide/en/integrate-scratch-pay-plans-with-third-party-services-fnFPz1e3De/Steps/2720498\nsummary:\n  types: [http]\n  scheme: bearer\n  note: >\n    The published Scratchpay partner/borrower API authenticates with a static\n    bearer token passed in the Authorization header (Authorization: Bearer <token>).\n    The specs declare this as an inline required header parameter rather than a formal\n    OpenAPI securityScheme, so the mechanical securityScheme deriver finds none; this\n    profile is captured from the spec parameters + the partner integration docs.\nschemes:\n  - name: partnerBearerToken\n    type: http\n    scheme: bearer\n    location: header\n    header_name: Authorization\n    format: 'Bearer <integration-token>'\n    token_provisioning: >\n      The integration token is issued to the practice/partner from the\
  \ Scratch\n      Dashboard (Account tab -> Integration Token, https://my.scratchpay.com/#/clinic/token).\n    sources:\n      - openapi/scratchpay-scratchpay-1.0.0-apis-swagger.yml\n      - openapi/scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml\n      - openapi/scratchpay-partner-1.0.0-apis-swagger.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/authentication/scratchpay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Financing
- Payments
- Lending
- Veterinary
- Healthcare
- Fintech
- Buy Now Pay Later
- Point of Sale
---
