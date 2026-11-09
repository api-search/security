---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aisle-wedding-dress-codes-api-openapi.yml
  format: yaml
  label: Aisle Dress codes API
  slug: aisle-wedding-dress-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-dress-codes-api-openapi.yml
- filename: aisle-wedding-events-api-openapi.yml
  format: yaml
  label: Aisle Events API
  slug: aisle-wedding-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-events-api-openapi.yml
- filename: aisle-wedding-guest-access-api-openapi.yml
  format: yaml
  label: Aisle Guest access API
  slug: aisle-wedding-guest-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-guest-access-api-openapi.yml
- filename: aisle-wedding-guest-content-api-openapi.yml
  format: yaml
  label: Aisle Guest content API
  slug: aisle-wedding-guest-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-guest-content-api-openapi.yml
- filename: aisle-wedding-guests-api-openapi.yml
  format: yaml
  label: Aisle Guests API
  slug: aisle-wedding-guests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-guests-api-openapi.yml
- filename: aisle-wedding-media-api-openapi.yml
  format: yaml
  label: Aisle Media API
  slug: aisle-wedding-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-media-api-openapi.yml
- filename: aisle-wedding-meta-api-openapi.yml
  format: yaml
  label: Aisle Meta API
  slug: aisle-wedding-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-meta-api-openapi.yml
- filename: aisle-wedding-parties-api-openapi.yml
  format: yaml
  label: Aisle Parties API
  slug: aisle-wedding-parties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-parties-api-openapi.yml
- filename: aisle-wedding-payments-api-openapi.yml
  format: yaml
  label: Aisle Payments API
  slug: aisle-wedding-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-payments-api-openapi.yml
- filename: aisle-wedding-payouts-api-openapi.yml
  format: yaml
  label: Aisle Payouts API
  slug: aisle-wedding-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-payouts-api-openapi.yml
- filename: aisle-wedding-recommendations-api-openapi.yml
  format: yaml
  label: Aisle Recommendations API
  slug: aisle-wedding-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-recommendations-api-openapi.yml
- filename: aisle-wedding-registry-api-openapi.yml
  format: yaml
  label: Aisle Registry API
  slug: aisle-wedding-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-registry-api-openapi.yml
- filename: aisle-wedding-rsvp-api-openapi.yml
  format: yaml
  label: Aisle RSVP API
  slug: aisle-wedding-rsvp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-rsvp-api-openapi.yml
- filename: aisle-wedding-site-api-openapi.yml
  format: yaml
  label: Aisle Site API
  slug: aisle-wedding-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-site-api-openapi.yml
- filename: aisle-wedding-statistics-api-openapi.yml
  format: yaml
  label: Aisle Statistics API
  slug: aisle-wedding-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-statistics-api-openapi.yml
- filename: aisle-wedding-stays-api-openapi.yml
  format: yaml
  label: Aisle Stays API
  slug: aisle-wedding-stays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-stays-api-openapi.yml
- filename: aisle-wedding-travel-api-openapi.yml
  format: yaml
  label: Aisle Travel API
  slug: aisle-wedding-travel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-travel-api-openapi.yml
- filename: aisle-wedding-wedding-api-openapi.yml
  format: yaml
  label: Aisle Wedding API
  slug: aisle-wedding-wedding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-wedding-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Aisle Wedding Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aisle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aisle
provider_slug: aisle-wedding
scheme_count: 1
schemes:
- description: A wedding-scoped API key. Send it from your own server; never from a browser.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aisle-wedding-openapi.json
  type: http
slug: aisle-wedding-authentication
source_filename: aisle-wedding-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/aisle-wedding-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A wedding-scoped API key. Send it from your own server; never from a browser.\n  sources:\n  - openapi/aisle-wedding-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aisle-wedding/authentication/aisle-wedding-authentication.yml
summary_line: http · 1 scheme
tags:
- Wedding
- Planning
- Software-as-a-Service
- Marketplace
---
