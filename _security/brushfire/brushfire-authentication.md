---
api_key_in:
- header
api_specs:
- filename: brushfire-accesscodes-api-openapi.yml
  format: yaml
  label: Brushfire AccessCodes API
  slug: brushfire-accesscodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-accesscodes-api-openapi.yml
- filename: brushfire-accounts-api-openapi.yml
  format: yaml
  label: Brushfire Accounts API
  slug: brushfire-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-accounts-api-openapi.yml
- filename: brushfire-attendees-api-openapi.yml
  format: yaml
  label: Brushfire Attendees API
  slug: brushfire-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-attendees-api-openapi.yml
- filename: brushfire-cart-api-openapi.yml
  format: yaml
  label: Brushfire Cart API
  slug: brushfire-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-cart-api-openapi.yml
- filename: brushfire-clients-api-openapi.yml
  format: yaml
  label: Brushfire Clients API
  slug: brushfire-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-clients-api-openapi.yml
- filename: brushfire-data-api-openapi.yml
  format: yaml
  label: Brushfire Data API
  slug: brushfire-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-data-api-openapi.yml
- filename: brushfire-events-api-openapi.yml
  format: yaml
  label: Brushfire Events API
  slug: brushfire-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-events-api-openapi.yml
- filename: brushfire-exchanges-api-openapi.yml
  format: yaml
  label: Brushfire Exchanges API
  slug: brushfire-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-exchanges-api-openapi.yml
- filename: brushfire-groups-api-openapi.yml
  format: yaml
  label: Brushfire Groups API
  slug: brushfire-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-groups-api-openapi.yml
- filename: brushfire-hooks-api-openapi.yml
  format: yaml
  label: Brushfire Hooks API
  slug: brushfire-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-hooks-api-openapi.yml
- filename: brushfire-lookups-api-openapi.yml
  format: yaml
  label: Brushfire Lookups API
  slug: brushfire-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-lookups-api-openapi.yml
- filename: brushfire-orders-api-openapi.yml
  format: yaml
  label: Brushfire Orders API
  slug: brushfire-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-orders-api-openapi.yml
- filename: brushfire-paymentprofiles-api-openapi.yml
  format: yaml
  label: Brushfire PaymentProfiles API
  slug: brushfire-paymentprofiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-paymentprofiles-api-openapi.yml
- filename: brushfire-promotions-api-openapi.yml
  format: yaml
  label: Brushfire Promotions API
  slug: brushfire-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-promotions-api-openapi.yml
- filename: brushfire-regions-api-openapi.yml
  format: yaml
  label: Brushfire Regions API
  slug: brushfire-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-regions-api-openapi.yml
- filename: brushfire-sessions-api-openapi.yml
  format: yaml
  label: Brushfire Sessions API
  slug: brushfire-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-sessions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Brushfire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brushfire secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brushfire
provider_slug: brushfire
scheme_count: 1
schemes:
- description: The App Key you received from https://developer.brushfire.com/key
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/brushfire-openapi.json
  type: apiKey
slug: brushfire-authentication
source_filename: brushfire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brushfire-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: The App Key you received from https://developer.brushfire.com/key\n  sources:\n  - openapi/brushfire-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/authentication/brushfire-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Event Ticketing
- Registration
- Event
- Ticketing
- Check-In
- Churches
- Payments
---
