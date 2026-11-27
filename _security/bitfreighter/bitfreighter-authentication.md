---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bitfreighter-edi-events-api-openapi.yml
  format: yaml
  label: Bitfreighter EDI Events API
  slug: bitfreighter-edi-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-edi-events-api-openapi.yml
- filename: bitfreighter-internal-api-openapi.yml
  format: yaml
  label: Bitfreighter Internal API
  slug: bitfreighter-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-internal-api-openapi.yml
- filename: bitfreighter-pricing-api-openapi.yml
  format: yaml
  label: Bitfreighter Pricing API
  slug: bitfreighter-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-pricing-api-openapi.yml
- filename: bitfreighter-real-time-rating-api-openapi.yml
  format: yaml
  label: Bitfreighter Real Time Rating API
  slug: bitfreighter-real-time-rating-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-real-time-rating-api-openapi.yml
- filename: bitfreighter-sending-edi-events-api-openapi.yml
  format: yaml
  label: Bitfreighter Sending EDI Events API
  slug: bitfreighter-sending-edi-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-sending-edi-events-api-openapi.yml
- filename: bitfreighter-spot-api-openapi.yml
  format: yaml
  label: Bitfreighter Spot API
  slug: bitfreighter-spot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-spot-api-openapi.yml
- filename: bitfreighter-webhooks-api-openapi.yml
  format: yaml
  label: Bitfreighter Webhooks API
  slug: bitfreighter-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitfreighter/openapi/bitfreighter-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bitfreighter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitfreighter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitfreighter
provider_slug: bitfreighter
scheme_count: 1
schemes:
- description: 'Bitfreighter APIs support OAuth 2.0 Client Credentials flow for authentication across all major endpoints.


    This is the **recommended authentication method** for new integrations, including both EDI and LiveQuote.


    These credentials can be obtained by reaching out to your Bitfreighter Customer Success representative.


    First, obtain an token from our authentication server. The authentication server'
  name: Bitfreighter OAuth
  scheme: bearer
  sources:
  - openapi/bitfreighter-openapi.yml
  type: http
slug: bitfreighter-authentication
source_filename: bitfreighter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/bitfreighter-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bitfreighter OAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bitfreighter APIs support OAuth 2.0 Client Credentials flow for authentication across all major endpoints.\n\n    This is the **recommended authentication method** for new integrations, including both EDI and LiveQuote.\n\n    These credentials can be obtained by reaching out to your Bitfreighter Customer Success representative.\n\n    First, obtain an token from our authentication server. The authentication server\n  sources:\n  - openapi/bitfreighter-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/bitfreighter/authentication/bitfreighter-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Freight
- EDI
- Logistics
---
