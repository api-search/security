---
api_key_in:
- header
api_specs:
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Reservations API
  slug: smoobu-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Apartments API
  slug: smoobu-apartments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Rates and Availability API
  slug: smoobu-rates-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Guests API
  slug: smoobu-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Messaging API
  slug: smoobu-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Webhooks
  slug: smoobu-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smoobu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smoobu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smoobu
provider_slug: smoobu
scheme_count: 1
schemes:
- description: Smoobu API key sent in the Api-Key header. HMAC-signed requests (X-API-Key / X-Timestamp / X-Nonce / X-Signature) are the recommended method; OAuth 2 is available for partners. The plain Api-Key header is documented as being sunset on 2026-09-25.
  in: header
  name: apiKey
  parameter: Api-Key
  sources:
  - openapi/smoobu-openapi.yml
  type: apiKey
slug: smoobu-authentication
source_filename: smoobu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smoobu-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Smoobu API key sent in the Api-Key header. HMAC-signed requests (X-API-Key /\n    X-Timestamp / X-Nonce / X-Signature) are the recommended method; OAuth 2 is available for\n    partners. The plain Api-Key header is documented as being sunset on 2026-09-25.\n  sources:\n  - openapi/smoobu-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/authentication/smoobu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vacation Rental
- Channel Manager
- Property Management
- Short-Term Rental
- Reservations
- Hospitality
---
