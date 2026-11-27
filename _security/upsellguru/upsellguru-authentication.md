---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: upsellguru-availability-api-openapi.yml
  format: yaml
  label: UpsellGuru Availability API
  slug: upsellguru-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-availability-api-openapi.yml
- filename: upsellguru-bookedextras-api-openapi.yml
  format: yaml
  label: UpsellGuru Booked Extras API
  slug: upsellguru-bookedextras-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-bookedextras-api-openapi.yml
- filename: upsellguru-extratypes-api-openapi.yml
  format: yaml
  label: UpsellGuru Extra Types API
  slug: upsellguru-extratypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-extratypes-api-openapi.yml
- filename: upsellguru-hotels-api-openapi.yml
  format: yaml
  label: UpsellGuru Hotels API
  slug: upsellguru-hotels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-hotels-api-openapi.yml
- filename: upsellguru-reservations-api-openapi.yml
  format: yaml
  label: UpsellGuru Reservations API
  slug: upsellguru-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-reservations-api-openapi.yml
- filename: upsellguru-roomtypes-api-openapi.yml
  format: yaml
  label: UpsellGuru Room Types API
  slug: upsellguru-roomtypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-roomtypes-api-openapi.yml
- filename: upsellguru-roomupgrades-api-openapi.yml
  format: yaml
  label: UpsellGuru Room Upgrades API
  slug: upsellguru-roomupgrades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-roomupgrades-api-openapi.yml
- filename: upsellguru-upgradebids-api-openapi.yml
  format: yaml
  label: UpsellGuru Upgrade Bids API
  slug: upsellguru-upgradebids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-upgradebids-api-openapi.yml
- filename: upsellguru-users-api-openapi.yml
  format: yaml
  label: UpsellGuru Users API
  slug: upsellguru-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upsellguru/openapi/upsellguru-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: UpsellGuru Authentication
name_suffix: Authentication
oauth_flows: []
overview: UpsellGuru secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UpsellGuru
provider_slug: upsellguru
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/upsellguru-openapi.yml
  type: apiKey
slug: upsellguru-authentication
source_filename: upsellguru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/upsellguru-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/upsellguru-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/upsellguru/authentication/upsellguru-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Hospitality
- Software-as-a-Service
- Revenue
- Upselling
---
