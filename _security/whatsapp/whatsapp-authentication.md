---
api_key_in: []
api_specs:
- filename: whatsapp-cloud-api-openapi.yml
  format: yaml
  label: WhatsApp Business Platform API
  slug: business-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-cloud-api-openapi.yml
- filename: whatsapp-business-management-api-openapi.yml
  format: yaml
  label: WhatsApp Business Account Management API
  slug: business-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-business-management-api-openapi.yml
- filename: whatsapp-flows-api-openapi.yml
  format: yaml
  label: WhatsApp Flows API
  slug: flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-flows-api-openapi.yml
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
