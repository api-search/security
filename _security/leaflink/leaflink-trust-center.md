---
api_specs:
- filename: leaflink-api-openapi-original.yml
  format: yaml
  label: LeafLink API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/openapi/leaflink-api-openapi-original.yml
- filename: leaflink-marketplace-v2-openapi-original.yml
  format: yaml
  label: LeafLink Marketplace V2 API
  slug: marketplace-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/openapi/leaflink-marketplace-v2-openapi-original.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Leaflink Trust Center
name_suffix: Trust Center
overview: LeafLink maintains a public trust center covering its security and compliance posture.
provider_name: LeafLink
provider_slug: leaflink
slug: leaflink-trust-center
source_filename: leaflink-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nurl: https://trust.leaflink.com/\npublished: true\ndiscovery: Linked as \"Trust Center\" from the leaflink.com primary navigation.\ncertifications: []\ncertifications_verified: false\nnote: LeafLink advertises a Trust Center at trust.leaflink.com from its main site navigation, but the host returns\n  HTTP 403 to both plain curl and a browser user-agent (bot protection). The page is therefore recorded as published\n  but its contents could not be read, and NO certifications are asserted. Because no certification could be verified,\n  no Compliance pointer is wired — re-probe on a later pass.\nevidence:\n- source: https://www.leaflink.com/\n  kind: navigation link\n  result: Trust Center -> https://trust.leaflink.com/\n- source: https://trust.leaflink.com/\n  kind: direct fetch\n  http_status: 403\n  user_agents_tried:\n  - curl\n  - Chrome 126 desktop\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/security/leaflink-trust-center.yml
summary_line: trust center published
tags:
- Cannabis
- Wholesale
- B2B Marketplace
- Supply Chain
- Payments
- Logistics
- Inventory
- Compliance
- Traceability
- eCommerce
- Distribution
- Retail
trust_url: https://trust.leaflink.com/
---
