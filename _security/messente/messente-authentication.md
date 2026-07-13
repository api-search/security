---
api_key_in: []
api_specs:
- filename: messente-openapi.yml
  format: yaml
  label: Messente Omnimessage API
  slug: messente-omnimessage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente SMS API
  slug: messente-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Contacts API
  slug: messente-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Groups API
  slug: messente-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Number Lookup API
  slug: messente-number-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Statistics API
  slug: messente-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
- filename: messente-openapi.yml
  format: yaml
  label: Messente Delivery Reports API
  slug: messente-delivery-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/openapi/messente-openapi.yml
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
