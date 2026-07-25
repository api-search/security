---
api_key_in:
- header
api_specs:
- filename: suger-api-api-openapi.yml
  format: yaml
  label: Suger API API
  slug: suger-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-api-api-openapi.yml
- filename: suger-billing-api-openapi.yml
  format: yaml
  label: Suger Billing API
  slug: suger-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-billing-api-openapi.yml
- filename: suger-buyer-api-openapi.yml
  format: yaml
  label: Suger Buyer API
  slug: suger-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-buyer-api-openapi.yml
- filename: suger-contact-api-openapi.yml
  format: yaml
  label: Suger Contact API
  slug: suger-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-contact-api-openapi.yml
- filename: suger-entitlement-api-openapi.yml
  format: yaml
  label: Suger Entitlement API
  slug: suger-entitlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-entitlement-api-openapi.yml
- filename: suger-metering-api-openapi.yml
  format: yaml
  label: Suger Metering API
  slug: suger-metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-metering-api-openapi.yml
- filename: suger-notification-api-openapi.yml
  format: yaml
  label: Suger Notification API
  slug: suger-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-notification-api-openapi.yml
- filename: suger-offer-api-openapi.yml
  format: yaml
  label: Suger Offer API
  slug: suger-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-offer-api-openapi.yml
- filename: suger-product-api-openapi.yml
  format: yaml
  label: Suger Product API
  slug: suger-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-product-api-openapi.yml
- filename: suger-report-api-openapi.yml
  format: yaml
  label: Suger Report API
  slug: suger-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-report-api-openapi.yml
- filename: suger-support-api-openapi.yml
  format: yaml
  label: Suger Support API
  slug: suger-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-support-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Suger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suger secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Suger
provider_slug: suger
scheme_count: 1
schemes:
- description: API Key for authorization in format of <Key *****>.
  in: header
  name: APIKeyAuth
  parameter: Authorization
  sources:
  - openapi/suger-openapi.yml
  type: apiKey
slug: suger-authentication
source_filename: suger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/suger-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API Key for authorization in format of <Key *****>.\n  sources:\n  - openapi/suger-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/authentication/suger-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Marketplace
- GTM
- SaaS
- Billing
- Entitlement
- Revenue
- Co-Sell
---
