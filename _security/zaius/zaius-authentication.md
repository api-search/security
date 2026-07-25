---
api_key_in:
- header
api_specs:
- filename: zaius-compliance-api-openapi.yml
  format: yaml
  label: Zaius Compliance API
  slug: zaius-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-compliance-api-openapi.yml
- filename: zaius-consent-api-openapi.yml
  format: yaml
  label: Zaius Consent API
  slug: zaius-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-consent-api-openapi.yml
- filename: zaius-consent-legacy-api-openapi.yml
  format: yaml
  label: Zaius Consent (Legacy) API
  slug: zaius-consent-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-consent-legacy-api-openapi.yml
- filename: zaius-customers-api-openapi.yml
  format: yaml
  label: Zaius Customers API
  slug: zaius-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-customers-api-openapi.yml
- filename: zaius-events-api-openapi.yml
  format: yaml
  label: Zaius Events API
  slug: zaius-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-events-api-openapi.yml
- filename: zaius-exports-api-openapi.yml
  format: yaml
  label: Zaius Exports API
  slug: zaius-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-exports-api-openapi.yml
- filename: zaius-fields-schema-api-openapi.yml
  format: yaml
  label: Zaius Fields schema API
  slug: zaius-fields-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-fields-schema-api-openapi.yml
- filename: zaius-identifiers-api-openapi.yml
  format: yaml
  label: Zaius Identifiers API
  slug: zaius-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-identifiers-api-openapi.yml
- filename: zaius-lists-api-openapi.yml
  format: yaml
  label: Zaius Lists API
  slug: zaius-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-lists-api-openapi.yml
- filename: zaius-object-schema-api-openapi.yml
  format: yaml
  label: Zaius Object schema API
  slug: zaius-object-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-object-schema-api-openapi.yml
- filename: zaius-objects-api-openapi.yml
  format: yaml
  label: Zaius Objects API
  slug: zaius-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-objects-api-openapi.yml
- filename: zaius-orders-api-openapi.yml
  format: yaml
  label: Zaius Orders API
  slug: zaius-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-orders-api-openapi.yml
- filename: zaius-products-api-openapi.yml
  format: yaml
  label: Zaius Products API
  slug: zaius-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-products-api-openapi.yml
- filename: zaius-reachability-api-openapi.yml
  format: yaml
  label: Zaius Reachability API
  slug: zaius-reachability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-reachability-api-openapi.yml
- filename: zaius-realtimesegments-api-openapi.yml
  format: yaml
  label: Zaius RealtimeSegments API
  slug: zaius-realtimesegments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-realtimesegments-api-openapi.yml
- filename: zaius-recommendations-api-openapi.yml
  format: yaml
  label: Zaius Recommendations API
  slug: zaius-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-recommendations-api-openapi.yml
- filename: zaius-relationships-schema-api-openapi.yml
  format: yaml
  label: Zaius Relationships schema API
  slug: zaius-relationships-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-relationships-schema-api-openapi.yml
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
