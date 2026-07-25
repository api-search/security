---
api_key_in:
- header
api_specs:
- filename: amazon-ad-groups-api-openapi.yml
  format: yaml
  label: Amazon Ad Groups API
  slug: amazon-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-ad-groups-api-openapi.yml
- filename: amazon-campaigns-api-openapi.yml
  format: yaml
  label: Amazon Campaigns API
  slug: amazon-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-campaigns-api-openapi.yml
- filename: amazon-catalog-api-openapi.yml
  format: yaml
  label: Amazon Catalog API
  slug: amazon-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-catalog-api-openapi.yml
- filename: amazon-charge-permissions-api-openapi.yml
  format: yaml
  label: Amazon Charge Permissions API
  slug: amazon-charge-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-charge-permissions-api-openapi.yml
- filename: amazon-charges-api-openapi.yml
  format: yaml
  label: Amazon Charges API
  slug: amazon-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-charges-api-openapi.yml
- filename: amazon-checkout-sessions-api-openapi.yml
  format: yaml
  label: Amazon Checkout Sessions API
  slug: amazon-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-checkout-sessions-api-openapi.yml
- filename: amazon-finances-api-openapi.yml
  format: yaml
  label: Amazon Finances API
  slug: amazon-finances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-finances-api-openapi.yml
- filename: amazon-inventory-api-openapi.yml
  format: yaml
  label: Amazon Inventory API
  slug: amazon-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-inventory-api-openapi.yml
- filename: amazon-keywords-api-openapi.yml
  format: yaml
  label: Amazon Keywords API
  slug: amazon-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-keywords-api-openapi.yml
- filename: amazon-listings-api-openapi.yml
  format: yaml
  label: Amazon Listings API
  slug: amazon-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-listings-api-openapi.yml
- filename: amazon-orders-api-openapi.yml
  format: yaml
  label: Amazon Orders API
  slug: amazon-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-orders-api-openapi.yml
- filename: amazon-profiles-api-openapi.yml
  format: yaml
  label: Amazon Profiles API
  slug: amazon-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-profiles-api-openapi.yml
- filename: amazon-refunds-api-openapi.yml
  format: yaml
  label: Amazon Refunds API
  slug: amazon-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-refunds-api-openapi.yml
- filename: amazon-reports-api-openapi.yml
  format: yaml
  label: Amazon Reports API
  slug: amazon-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-reports-api-openapi.yml
- filename: amazon-targets-api-openapi.yml
  format: yaml
  label: Amazon Targets API
  slug: amazon-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-targets-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Amazon
provider_slug: amazon
scheme_count: 2
schemes:
- description: OAuth 2.0 access token from Login with Amazon
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/amazon-advertising-api-openapi.yml
  - openapi/amazon-selling-partner-api-openapi.yml
  type: http
- description: AMZN-PAY-RSASSA-PSS-V2 signature using merchant private key
  in: header
  name: amazonPaySignature
  parameter: authorization
  sources:
  - openapi/amazon-pay-api-openapi.yml
  type: apiKey
slug: amazon-authentication
source_filename: amazon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-advertising-api-openapi.yml, openapi/amazon-pay-api-openapi.yml, openapi/amazon-selling-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token from Login with Amazon\n  sources:\n  - openapi/amazon-advertising-api-openapi.yml\n  - openapi/amazon-selling-partner-api-openapi.yml\n- name: amazonPaySignature\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: AMZN-PAY-RSASSA-PSS-V2 signature using merchant private key\n  sources:\n  - openapi/amazon-pay-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/authentication/amazon-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
- Fortune 100
---
