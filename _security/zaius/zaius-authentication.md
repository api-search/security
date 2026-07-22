---
api_key_in:
- header
api_specs:
- filename: zaius-events-openapi.json
  format: json
  label: ODP Events API
  slug: odp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-events-openapi.json
- filename: zaius-customers-openapi.json
  format: json
  label: ODP Customers API
  slug: odp-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-customers-openapi.json
- filename: zaius-orders-openapi.json
  format: json
  label: ODP Orders API
  slug: odp-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-orders-openapi.json
- filename: zaius-products-openapi.json
  format: json
  label: ODP Products API
  slug: odp-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-products-openapi.json
- filename: zaius-objects-openapi.json
  format: json
  label: ODP Objects API
  slug: odp-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-objects-openapi.json
- filename: zaius-lists-openapi.json
  format: json
  label: ODP Lists API
  slug: odp-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-lists-openapi.json
- filename: zaius-consent-openapi.json
  format: json
  label: ODP Consent API
  slug: odp-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-consent-openapi.json
- filename: zaius-exports-openapi.json
  format: json
  label: ODP Exports API
  slug: odp-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-exports-openapi.json
- filename: zaius-recommendations-openapi.json
  format: json
  label: ODP Recommendations API
  slug: odp-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-recommendations-openapi.json
- filename: zaius-realtimesegments-openapi.json
  format: json
  label: ODP Real-Time Segments API
  slug: odp-real-time-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-realtimesegments-openapi.json
- filename: zaius-advanced-openapi.json
  format: json
  label: ODP Advanced API (schema, identifiers, compliance)
  slug: odp-advanced-api-schema-identifiers-compliance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-advanced-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Zaius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zaius secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zaius
provider_slug: zaius
scheme_count: 1
schemes:
- in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/zaius-advanced-openapi.json
  - openapi/zaius-consent-openapi.json
  - openapi/zaius-customers-openapi.json
  - openapi/zaius-events-openapi.json
  - openapi/zaius-exports-openapi.json
  - openapi/zaius-lists-openapi.json
  - openapi/zaius-objects-openapi.json
  - openapi/zaius-orders-openapi.json
  - openapi/zaius-products-openapi.json
  - openapi/zaius-realtimesegments-openapi.json
  - openapi/zaius-recommendations-openapi.json
  type: apiKey
slug: zaius-authentication
source_filename: zaius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.developers.optimizely.com/optimizely-data-platform/reference/authentication\ndocs: https://docs.developers.optimizely.com/optimizely-data-platform/reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nkey_types:\n- name: public\n  alias: Tracker ID\n  use: most data-send calls and limited, publicly-exposable retrieval calls\n- name: private\n  use: querying ODP data from trusted backend services and integrations\n  revocation_grace: revoked private keys remain valid for a 12-hour grace period\nkey_location: ODP UI Settings > APIs (lists public + private keys with usage plans and rate limits)\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/zaius-advanced-openapi.json\n  - openapi/zaius-consent-openapi.json\n  - openapi/zaius-customers-openapi.json\n  - openapi/zaius-events-openapi.json\n  - openapi/zaius-exports-openapi.json\n\
  \  - openapi/zaius-lists-openapi.json\n  - openapi/zaius-objects-openapi.json\n  - openapi/zaius-orders-openapi.json\n  - openapi/zaius-products-openapi.json\n  - openapi/zaius-realtimesegments-openapi.json\n  - openapi/zaius-recommendations-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/authentication/zaius-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Customer Data Platform
- CDP
- Marketing
- Personalization
- Segmentation
- Ecommerce
- Customer Data
- Real-Time Audiences
- Events
---
