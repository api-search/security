---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nextdc-comments-api-openapi.yml
  format: yaml
  label: NEXTDC Comments API
  slug: nextdc-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-comments-api-openapi.yml
- filename: nextdc-discount-api-openapi.yml
  format: yaml
  label: NEXTDC Discount API
  slug: nextdc-discount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-discount-api-openapi.yml
- filename: nextdc-discounts-api-openapi.yml
  format: yaml
  label: NEXTDC Discounts API
  slug: nextdc-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-discounts-api-openapi.yml
- filename: nextdc-limitations-api-openapi.yml
  format: yaml
  label: NEXTDC Limitations API
  slug: nextdc-limitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-limitations-api-openapi.yml
- filename: nextdc-locations-api-openapi.yml
  format: yaml
  label: NEXTDC Locations API
  slug: nextdc-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-locations-api-openapi.yml
- filename: nextdc-pricepoints-api-openapi.yml
  format: yaml
  label: NEXTDC Pricepoints API
  slug: nextdc-pricepoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-pricepoints-api-openapi.yml
- filename: nextdc-quote-api-openapi.yml
  format: yaml
  label: NEXTDC Quote API
  slug: nextdc-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-quote-api-openapi.yml
- filename: nextdc-quotes-api-openapi.yml
  format: yaml
  label: NEXTDC Quotes API
  slug: nextdc-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-quotes-api-openapi.yml
- filename: nextdc-resource-api-openapi.yml
  format: yaml
  label: NEXTDC Resource API
  slug: nextdc-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-resource-api-openapi.yml
- filename: nextdc-resources-api-openapi.yml
  format: yaml
  label: NEXTDC Resources API
  slug: nextdc-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-resources-api-openapi.yml
- filename: nextdc-service-api-openapi.yml
  format: yaml
  label: NEXTDC Service API
  slug: nextdc-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-service-api-openapi.yml
- filename: nextdc-services-api-openapi.yml
  format: yaml
  label: NEXTDC Services API
  slug: nextdc-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-services-api-openapi.yml
- filename: nextdc-task-api-openapi.yml
  format: yaml
  label: NEXTDC Task API
  slug: nextdc-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-task-api-openapi.yml
- filename: nextdc-tasks-api-openapi.yml
  format: yaml
  label: NEXTDC Tasks API
  slug: nextdc-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-tasks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Nextdc Authentication
name_suffix: Authentication
oauth_flows: []
overview: NEXTDC secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NEXTDC
provider_slug: nextdc
scheme_count: 2
schemes:
- clock_skew: Clients need to ensure that the nonce time is accurate to within 2 minutes of the API server time otherwise authentication will fail.
  companion_headers:
  - name: X-API-TS
    purpose: nonce (unix timestamp with millisecond or better resolution, e.g. date '+%s.%N')
  format: key:digest
  in: header
  ip_allowlist: true
  name: axon_hmac_api_key
  parameter: X-API-Key
  provisioning: Please speak to your pre-sales representative to request API access and the process to obtain an API key and sandbox access. You will need to supply an existing AXON user that you wish to grant API access to and the source IP addresses that you will be accessing the API from.
  replay_protection: The AXON API requires an increasing, never repeated nonce to guard against replay attacks.
  signature:
    algorithm: HMAC-SHA256
    encoding: hex (the digest is not base64 encoded)
    signed_string: method + path (query parameters excluded) + nonce, no spaces
  sources:
  - https://www.nextdc.com/knowledge-articles/axon-api-documentation
  type: apiKey
- in: query
  name: api_key
  note: Declared in the Swagger 2.0 contract (openapi/nextdc-axon-openapi.yml); the docs describe the header-based HMAC scheme above instead.
  parameter: api_key
  sources:
  - openapi/nextdc-axon-openapi.yml
  type: apiKey
slug: nextdc-authentication
source_filename: nextdc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://www.nextdc.com/knowledge-articles/axon-api-documentation\ndocs: https://www.nextdc.com/knowledge-articles/axon-api-documentation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  signed_requests: true\nschemes:\n- name: axon_hmac_api_key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  format: 'key:digest'\n  companion_headers:\n  - name: X-API-TS\n    purpose: nonce (unix timestamp with millisecond or better resolution, e.g. date '+%s.%N')\n  signature:\n    algorithm: HMAC-SHA256\n    signed_string: method + path (query parameters excluded) + nonce, no spaces\n    encoding: hex (the digest is not base64 encoded)\n  replay_protection: 'The AXON API requires an increasing, never repeated nonce to guard against replay attacks.'\n  clock_skew: 'Clients need to ensure that the nonce time is accurate to within 2 minutes of the API server time otherwise authentication will fail.'\n  provisioning: 'Please\
  \ speak to your pre-sales representative to request API access and the process to obtain an API key and sandbox access. You will need to supply an existing AXON user that you wish to grant API access to and the source IP addresses that you will be accessing the API from.'\n  ip_allowlist: true\n  sources:\n  - https://www.nextdc.com/knowledge-articles/axon-api-documentation\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  note: Declared in the Swagger 2.0 contract (openapi/nextdc-axon-openapi.yml); the docs describe the header-based HMAC scheme above instead.\n  sources:\n  - openapi/nextdc-axon-openapi.yml\nauthorization_model: 'The company access control model in AXON is hierarchical. This means that having access at a specific level in the hierarchy,access flows down to sub-companies.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/authentication/nextdc-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Data Centers
- Colocation
- Cloud Infrastructure
- Connectivity
- Artificial Intelligence
- Australia
---
