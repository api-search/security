---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: vincario-vin-decoder-api-openapi.yml
  format: yaml
  label: Vincario VIN Decoder API
  slug: vincario-vin-decoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-vin-decoder-api-openapi.yml
- filename: vincario-oem-vin-lookup-api-openapi.yml
  format: yaml
  label: Vincario OEM VIN Lookup API
  slug: vincario-oem-vin-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-oem-vin-lookup-api-openapi.yml
- filename: vincario-oem-service-history-api-openapi.yml
  format: yaml
  label: Vincario OEM Service History API
  slug: vincario-oem-service-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-oem-service-history-api-openapi.yml
- filename: vincario-vehicle-market-value-api-openapi.yml
  format: yaml
  label: Vincario Vehicle Market Value API
  slug: vincario-vehicle-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-vehicle-market-value-api-openapi.yml
- filename: vincario-stolen-check-api-openapi.yml
  format: yaml
  label: Vincario Stolen Check API
  slug: vincario-stolen-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-stolen-check-api-openapi.yml
- filename: vincario-get-balance-api-openapi.yml
  format: yaml
  label: Vincario Credit Balance API
  slug: vincario-get-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-get-balance-api-openapi.yml
- filename: vincario-enums-api-openapi.yml
  format: yaml
  label: Vincario Enums API
  slug: vincario-enums-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/openapi/vincario-enums-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Vincario Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vincario secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vincario
provider_slug: vincario
scheme_count: 1
schemes:
- description: Path-signed authentication. The API key (id) and a per-request SHA1 control sum are passed as URL path segments rather than headers or query parameters; this scheme is declared as a placeholder because OpenAPI 3.0 cannot natively express path-segment-based signed credentials. The control sum is `substr(sha1("{lookup}|{id}|{apikey}|{secretkey}"), 0, 10)`. The secret key is never sent over the wire.
  in: query
  name: signedPath
  parameter: controlsum
  sources:
  - openapi/vincario-openapi.yml
  type: apiKey
slug: vincario-authentication
source_filename: vincario-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vincario-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: signedPath\n  type: apiKey\n  in: query\n  parameter: controlsum\n  description: Path-signed authentication. The API key (id) and a per-request SHA1 control sum\n    are passed as URL path segments rather than headers or query parameters; this scheme is\n    declared as a placeholder because OpenAPI 3.0 cannot natively express path-segment-based\n    signed credentials. The control sum is `substr(sha1(\"{lookup}|{id}|{apikey}|{secretkey}\"),\n    0, 10)`. The secret key is never sent over the wire.\n  sources:\n  - openapi/vincario-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vincario/refs/heads/main/authentication/vincario-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- VIN
- Vehicle Data
- Automotive
- VIN Decoder
- Market Value
---
