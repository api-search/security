---
anonymous_access: false
api_key_in: []
api_specs:
- filename: withlocals-availability-api-openapi.yml
  format: yaml
  label: Withlocals Availability API
  slug: withlocals-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-availability-api-openapi.yml
- filename: withlocals-bookings-api-openapi.yml
  format: yaml
  label: Withlocals Bookings API
  slug: withlocals-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-bookings-api-openapi.yml
- filename: withlocals-products-api-openapi.yml
  format: yaml
  label: Withlocals Products API
  slug: withlocals-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-products-api-openapi.yml
- filename: withlocals-supplier-api-openapi.yml
  format: yaml
  label: Withlocals Supplier API
  slug: withlocals-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-supplier-api-openapi.yml
- filename: withlocals-webhooks-api-openapi.yml
  format: yaml
  label: Withlocals Webhooks API
  slug: withlocals-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Withlocals Authentication
name_suffix: Authentication
oauth_flows: []
overview: Withlocals secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Withlocals
provider_slug: withlocals
scheme_count: 1
schemes:
- bearerFormat: opaque
  description: "Per-partner opaque API token issued by Withlocals. Send on every\nrequest as:\n\n    Authorization: Bearer <token>"
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/withlocals-partner-api-openapi.yml
  type: http
slug: withlocals-authentication
source_filename: withlocals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/withlocals-partner-api-openapi.yml\ndocs: https://developers.withlocals.com/api-reference/\nprobed: \"GET https://test-api.withlocals.com/v1/partner/products without a token returned HTTP 401 (2026-10-09)\"\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: |-\n    Per-partner opaque API token issued by Withlocals. Send on every\n    request as:\n\n        Authorization: Bearer <token>\n  sources:\n  - openapi/withlocals-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/authentication/withlocals-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Travel
- Tours
- Experiences
- Tourism
- Marketplace
- Partner API
---
