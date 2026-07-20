---
api_key_in:
- header
api_specs:
- filename: liquidonate-magicmatch-openapi.yml
  format: yaml
  label: MagicMatch by LiquiDonate
  slug: magicmatch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/openapi/liquidonate-magicmatch-openapi.yml
- filename: liquidonate-returnsdirect-openapi.yml
  format: yaml
  label: ReturnsDirect by LiquiDonate (Beta)
  slug: returnsdirect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/openapi/liquidonate-returnsdirect-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Liquidonate Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiquiDonate secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LiquiDonate
provider_slug: liquidonate
scheme_count: 4
schemes:
- description: Retailer API key issued by v1/setupRetailer. Prefixed `ld_`.
  in: header
  name: liquidonateKey
  parameter: X-LiquiDonate-Key
  sources:
  - openapi/liquidonate-magicmatch-openapi.yml
  type: apiKey
- description: Retailer API secret issued by v1/setupRetailer. Prefixed `ld_sk_`.
  in: header
  name: liquidonateSecret
  parameter: X-LiquiDonate-Secret
  sources:
  - openapi/liquidonate-magicmatch-openapi.yml
  type: apiKey
- description: Your shop identifier, e.g. acme.com. Must match the value LiquiDonate has on file.
  in: header
  name: shopDomain
  parameter: X-Shop-Domain
  sources:
  - openapi/liquidonate-returnsdirect-openapi.yml
  type: apiKey
- description: HMAC-SHA256 of the raw request body using the shared secret LiquiDonate provisions for your shop, as lowercase hex.
  in: header
  name: hmacSignature
  parameter: X-Signature
  sources:
  - openapi/liquidonate-returnsdirect-openapi.yml
  type: apiKey
slug: liquidonate-authentication
source_filename: liquidonate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/liquidonate-magicmatch-openapi.yml, openapi/liquidonate-returnsdirect-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: liquidonateKey\n  type: apiKey\n  in: header\n  parameter: X-LiquiDonate-Key\n  description: Retailer API key issued by v1/setupRetailer. Prefixed `ld_`.\n  sources:\n  - openapi/liquidonate-magicmatch-openapi.yml\n- name: liquidonateSecret\n  type: apiKey\n  in: header\n  parameter: X-LiquiDonate-Secret\n  description: Retailer API secret issued by v1/setupRetailer. Prefixed `ld_sk_`.\n  sources:\n  - openapi/liquidonate-magicmatch-openapi.yml\n- name: shopDomain\n  type: apiKey\n  in: header\n  parameter: X-Shop-Domain\n  description: Your shop identifier, e.g. acme.com. Must match the value LiquiDonate has on\n    file.\n  sources:\n  - openapi/liquidonate-returnsdirect-openapi.yml\n- name: hmacSignature\n  type: apiKey\n  in: header\n  parameter: X-Signature\n\
  \  description: HMAC-SHA256 of the raw request body using the shared secret LiquiDonate provisions\n    for your shop, as lowercase hex.\n  sources:\n  - openapi/liquidonate-returnsdirect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/authentication/liquidonate-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Reverse Logistics
- Returns Management
- Donations
- Nonprofits
- Retail
- Ecommerce
- Sustainability
- Circular Economy
- Shipping
- Supply Chain
- Excess Inventory
- Company
---
