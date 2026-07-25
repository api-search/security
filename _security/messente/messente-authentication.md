---
api_key_in: []
api_specs:
- filename: messente-account-balance-api-openapi.yml
  format: yaml
  label: Messente Account Balance API
  slug: messente-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-account-balance-api-openapi.yml
- filename: messente-blacklist-api-openapi.yml
  format: yaml
  label: Messente Blacklist API
  slug: messente-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-blacklist-api-openapi.yml
- filename: messente-bulk-messaging-api-openapi.yml
  format: yaml
  label: Messente Bulk Messaging API
  slug: messente-bulk-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-bulk-messaging-api-openapi.yml
- filename: messente-contacts-api-openapi.yml
  format: yaml
  label: Messente Contacts API
  slug: messente-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-contacts-api-openapi.yml
- filename: messente-delivery-report-api-openapi.yml
  format: yaml
  label: Messente Delivery Report API
  slug: messente-delivery-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-delivery-report-api-openapi.yml
- filename: messente-groups-api-openapi.yml
  format: yaml
  label: Messente Groups API
  slug: messente-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-groups-api-openapi.yml
- filename: messente-number-lookup-api-openapi.yml
  format: yaml
  label: Messente Number Lookup API
  slug: messente-number-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-number-lookup-api-openapi.yml
- filename: messente-number-verification-api-openapi.yml
  format: yaml
  label: Messente Number Verification API
  slug: messente-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-number-verification-api-openapi.yml
- filename: messente-omnimessage-api-openapi.yml
  format: yaml
  label: Messente Omnimessage API
  slug: messente-omnimessage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-omnimessage-api-openapi.yml
- filename: messente-pricing-api-openapi.yml
  format: yaml
  label: Messente Pricing API
  slug: messente-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-pricing-api-openapi.yml
- filename: messente-statistics-api-openapi.yml
  format: yaml
  label: Messente Statistics API
  slug: messente-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-statistics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Messente Authentication
name_suffix: Authentication
oauth_flows: []
overview: Messente secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Messente
provider_slug: messente
scheme_count: 1
schemes:
- description: HTTP Basic authentication using the API username and password from the Messente dashboard API settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/messente-openapi.yml
  type: http
slug: messente-authentication
source_filename: messente-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/messente-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the API username and password from the Messente\n    dashboard API settings.\n  sources:\n  - openapi/messente-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/authentication/messente-authentication.yml
summary_line: http · 1 scheme
tags:
- CPaaS
- Messaging
- SMS
- Viber
- WhatsApp
- Verification
- 2FA
---
