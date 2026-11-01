---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ometria-contacts-api-openapi.yml
  format: yaml
  label: Ometria Contacts API
  slug: ometria-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-contacts-api-openapi.yml
- filename: ometria-custom-event-api-openapi.yml
  format: yaml
  label: Ometria Custom Event API
  slug: ometria-custom-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-custom-event-api-openapi.yml
- filename: ometria-custom-fields-api-openapi.yml
  format: yaml
  label: Ometria Custom Fields API
  slug: ometria-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-custom-fields-api-openapi.yml
- filename: ometria-field-forget-email-phone-erasure-api-openapi.yml
  format: yaml
  label: Ometria Field forget (email / phone erasure) API
  slug: ometria-field-forget-email-phone-erasure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-field-forget-email-phone-erasure-api-openapi.yml
- filename: ometria-gdpr-anonymisation-requests-api-openapi.yml
  format: yaml
  label: Ometria GDPR anonymisation requests API
  slug: ometria-gdpr-anonymisation-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-gdpr-anonymisation-requests-api-openapi.yml
- filename: ometria-lists-api-openapi.yml
  format: yaml
  label: Ometria Lists API
  slug: ometria-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-lists-api-openapi.yml
- filename: ometria-orders-api-openapi.yml
  format: yaml
  label: Ometria Orders API
  slug: ometria-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-orders-api-openapi.yml
- filename: ometria-products-api-openapi.yml
  format: yaml
  label: Ometria Products API
  slug: ometria-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-products-api-openapi.yml
- filename: ometria-profiles-api-openapi.yml
  format: yaml
  label: Ometria Profiles API
  slug: ometria-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-profiles-api-openapi.yml
- filename: ometria-push-api-openapi.yml
  format: yaml
  label: Ometria Push API
  slug: ometria-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-push-api-openapi.yml
- filename: ometria-transactional-email-api-openapi.yml
  format: yaml
  label: Ometria Transactional Email API
  slug: ometria-transactional-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-transactional-email-api-openapi.yml
- filename: ometria-translation-requests-api-openapi.yml
  format: yaml
  label: Ometria Translation Requests API
  slug: ometria-translation-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-translation-requests-api-openapi.yml
- filename: ometria-unsubscribes-api-openapi.yml
  format: yaml
  label: Ometria Unsubscribes API
  slug: ometria-unsubscribes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-unsubscribes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ometria Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ometria secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ometria
provider_slug: ometria
scheme_count: 1
schemes:
- description: Ometria API key which can be obtained from your Ometria account administrator
  in: header
  name: apikey
  parameter: X-Ometria-Auth
  sources:
  - openapi/ometria-data-api-openapi.yml
  type: apiKey
slug: ometria-authentication
source_filename: ometria-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/ometria-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: X-Ometria-Auth\n  description: Ometria API key which can be obtained from your Ometria account administrator\n  sources:\n  - openapi/ometria-data-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/ometria/authentication/ometria-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Retail
- Customer Data Platform
- AI
- Marketing
---
