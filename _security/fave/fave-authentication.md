---
api_key_in:
- query
api_specs:
- filename: fave-favepay-omni-openapi.yml
  format: yaml
  label: FavePay Omni (FPO) API
  slug: favepay-omni-fpo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fave/refs/heads/main/openapi/fave-favepay-omni-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fave secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fave
provider_slug: fave
scheme_count: 1
schemes:
- description: HMAC-SHA256 signature computed over the URL-encoded request fields in submission order (excluding sign and country_code, and excluding outlet_id on list, id on acknowledge, and details on merchant scan), keyed by the secret Fave issued for the integration. On POST requests the signature is passed as the sign field in the request body.
  in: query
  name: hmacSignature
  parameter: sign
  sources:
  - openapi/fave-favepay-omni-openapi.yml
  type: apiKey
slug: fave-authentication
source_filename: fave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fave-favepay-omni-openapi.yml\ndocs: https://developers.myfave.com/fpo-guide.html\nmodel: >-\n  Request signing (not a bearer/OAuth scheme). Every request is signed with\n  HMAC-SHA256 using the secret key Fave issues per integration during partner\n  onboarding. The signing string is the URL-encoded request fields in submission\n  order (never alphabetical), excluding `sign` and `country_code`, plus\n  `outlet_id` on list, `id` on acknowledge, and `details` on merchant scan. The\n  computed digest is passed as `sign` (query param on GET, body field on POST).\n  Webhook callbacks carry the same `sign` field and must be verified before use.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: hmacSignature\n  type: apiKey\n  in: query\n  parameter: sign\n  description: HMAC-SHA256 signature computed over the URL-encoded request fields in submission\n    order (excluding sign and country_code,\
  \ and excluding outlet_id on list, id on acknowledge,\n    and details on merchant scan), keyed by the secret Fave issued for the integration. On POST\n    requests the signature is passed as the sign field in the request body.\n  sources:\n  - openapi/fave-favepay-omni-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fave/refs/heads/main/authentication/fave-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Payments
- Fintech
- QR Payments
- Loyalty
- Cashback
- Merchant Services
- Southeast Asia
- Webhooks
---
