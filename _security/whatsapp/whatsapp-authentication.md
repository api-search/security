---
api_key_in: []
api_specs:
- filename: whatsapp-flows-api-openapi.yml
  format: yaml
  label: WhatsApp Flows API
  slug: flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-flows-api-openapi.yml
- filename: whatsapp-on-premises-api-deprecated
  format: yaml
  label: WhatsApp On-Premises API
  slug: on-premises-api
  spec_type: Postman
  url: https://www.postman.com/meta/whatsapp-business-platform/collection/vdi189b/whatsapp-on-premises-api-deprecated
- filename: whatsapp-analytics-api-openapi.yml
  format: yaml
  label: WhatsApp Analytics API
  slug: whatsapp-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-analytics-api-openapi.yml
- filename: whatsapp-assets-api-openapi.yml
  format: yaml
  label: WhatsApp Assets API
  slug: whatsapp-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-assets-api-openapi.yml
- filename: whatsapp-assigned-users-api-openapi.yml
  format: yaml
  label: WhatsApp Assigned Users API
  slug: whatsapp-assigned-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-assigned-users-api-openapi.yml
- filename: whatsapp-business-accounts-api-openapi.yml
  format: yaml
  label: WhatsApp Business Accounts API
  slug: whatsapp-business-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-business-accounts-api-openapi.yml
- filename: whatsapp-business-profile-api-openapi.yml
  format: yaml
  label: WhatsApp Business Profile API
  slug: whatsapp-business-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-business-profile-api-openapi.yml
- filename: whatsapp-lifecycle-api-openapi.yml
  format: yaml
  label: WhatsApp Lifecycle API
  slug: whatsapp-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-lifecycle-api-openapi.yml
- filename: whatsapp-media-api-openapi.yml
  format: yaml
  label: WhatsApp Media API
  slug: whatsapp-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-media-api-openapi.yml
- filename: whatsapp-message-templates-api-openapi.yml
  format: yaml
  label: WhatsApp Message Templates API
  slug: whatsapp-message-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-message-templates-api-openapi.yml
- filename: whatsapp-messages-api-openapi.yml
  format: yaml
  label: WhatsApp Messages API
  slug: whatsapp-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-messages-api-openapi.yml
- filename: whatsapp-phone-numbers-api-openapi.yml
  format: yaml
  label: WhatsApp Phone Numbers API
  slug: whatsapp-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-phone-numbers-api-openapi.yml
- filename: whatsapp-product-catalogs-api-openapi.yml
  format: yaml
  label: WhatsApp Product Catalogs API
  slug: whatsapp-product-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-product-catalogs-api-openapi.yml
- filename: whatsapp-qr-codes-api-openapi.yml
  format: yaml
  label: WhatsApp QR Codes API
  slug: whatsapp-qr-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-qr-codes-api-openapi.yml
- filename: whatsapp-registration-api-openapi.yml
  format: yaml
  label: WhatsApp Registration API
  slug: whatsapp-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-registration-api-openapi.yml
- filename: whatsapp-subscribed-apps-api-openapi.yml
  format: yaml
  label: WhatsApp Subscribed Apps API
  slug: whatsapp-subscribed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-subscribed-apps-api-openapi.yml
- filename: whatsapp-two-step-verification-api-openapi.yml
  format: yaml
  label: WhatsApp Two-Step Verification API
  slug: whatsapp-two-step-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-two-step-verification-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Whatsapp Authentication
name_suffix: Authentication
oauth_flows: []
overview: WhatsApp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WhatsApp
provider_slug: whatsapp
scheme_count: 1
schemes:
- description: System User Token with whatsapp_business_management permission
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/whatsapp-business-management-api-openapi.yml
  - openapi/whatsapp-cloud-api-openapi.yml
  - openapi/whatsapp-flows-api-openapi.yml
  type: http
slug: whatsapp-authentication
source_filename: whatsapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whatsapp-business-management-api-openapi.yml, openapi/whatsapp-cloud-api-openapi.yml,\n  openapi/whatsapp-flows-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: System User Token with whatsapp_business_management permission\n  sources:\n  - openapi/whatsapp-business-management-api-openapi.yml\n  - openapi/whatsapp-cloud-api-openapi.yml\n  - openapi/whatsapp-flows-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/authentication/whatsapp-authentication.yml
summary_line: http · 1 scheme
tags: []
---
