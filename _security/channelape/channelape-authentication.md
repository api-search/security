---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: channelape-openapi-generated.yml
  format: yaml
  label: ChannelApe API
  slug: channelape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/_ae-authored/channelape-openapi-generated.yml
- filename: channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api-openapi.yml
  format: yaml
  label: ChannelApe 0B2D6F2B 4676 40B4 9588 2A4C93F6B250 API
  slug: channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api-openapi.yml
- filename: channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api-openapi.yml
  format: yaml
  label: ChannelApe 6F7402B4 E75C 4573 B3B4 3139Dc1B733D API
  slug: channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api-openapi.yml
- filename: channelape-channelape-api-api-openapi.yml
  format: yaml
  label: ChannelApe ChannelApe API
  slug: channelape-channelape-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-channelape-api-api-openapi.yml
- filename: channelape-inventory-item-quantity-adjustments-api-openapi.yml
  format: yaml
  label: ChannelApe Inventory Item Quantity Adjustments API
  slug: channelape-inventory-item-quantity-adjustments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-inventory-item-quantity-adjustments-api-openapi.yml
- filename: channelape-rest-api-openapi.yml
  format: yaml
  label: ChannelApe Rest API
  slug: channelape-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-rest-api-openapi.yml
- filename: channelape-suppliers-api-openapi.yml
  format: yaml
  label: ChannelApe Suppliers API
  slug: channelape-suppliers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-suppliers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Channelape Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChannelApe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ChannelApe
provider_slug: channelape
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api-openapi.yml
  - openapi/channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api-openapi.yml
  - openapi/channelape-channelape-api-api-openapi.yml
  - openapi/channelape-inventory-item-quantity-adjustments-api-openapi.yml
  - openapi/channelape-rest-api-openapi.yml
  - openapi/channelape-suppliers-api-openapi.yml
  type: apiKey
slug: channelape-authentication
source_filename: channelape-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api-openapi.yml, openapi/channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api-openapi.yml,\n  openapi/channelape-channelape-api-api-openapi.yml, openapi/channelape-inventory-item-quantity-adjustments-api-openapi.yml,\n  openapi/channelape-rest-api-openapi.yml, openapi/channelape-suppliers-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api-openapi.yml\n  - openapi/channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api-openapi.yml\n  - openapi/channelape-channelape-api-api-openapi.yml\n  - openapi/channelape-inventory-item-quantity-adjustments-api-openapi.yml\n  - openapi/channelape-rest-api-openapi.yml\n  - openapi/channelape-suppliers-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/channelape/authentication/channelape-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Inventory
- Wholesale
- Retail
---
