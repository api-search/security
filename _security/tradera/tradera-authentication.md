---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: tradera-auth-api-openapi.yml
  format: yaml
  label: Tradera Auth API
  slug: tradera-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-auth-api-openapi.yml
- filename: tradera-buyer-api-openapi.yml
  format: yaml
  label: Tradera Buyer API
  slug: tradera-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-buyer-api-openapi.yml
- filename: tradera-categories-api-openapi.yml
  format: yaml
  label: Tradera Categories API
  slug: tradera-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-categories-api-openapi.yml
- filename: tradera-items-api-openapi.yml
  format: yaml
  label: Tradera Items API
  slug: tradera-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-items-api-openapi.yml
- filename: tradera-listings-api-openapi.yml
  format: yaml
  label: Tradera Listings API
  slug: tradera-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-listings-api-openapi.yml
- filename: tradera-orders-api-openapi.yml
  format: yaml
  label: Tradera Orders API
  slug: tradera-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-orders-api-openapi.yml
- filename: tradera-program-api-openapi.yml
  format: yaml
  label: Tradera Program API
  slug: tradera-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-program-api-openapi.yml
- filename: tradera-reference-data-api-openapi.yml
  format: yaml
  label: Tradera Reference Data API
  slug: tradera-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-reference-data-api-openapi.yml
- filename: tradera-search-api-openapi.yml
  format: yaml
  label: Tradera Search API
  slug: tradera-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-search-api-openapi.yml
- filename: tradera-tradera-api-services-core-api-openapi.yml
  format: yaml
  label: Tradera Tradera.Api.Services.Core API
  slug: tradera-tradera-api-services-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-tradera-api-services-core-api-openapi.yml
- filename: tradera-users-api-openapi.yml
  format: yaml
  label: Tradera Users API
  slug: tradera-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Tradera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tradera secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tradera
provider_slug: tradera
scheme_count: 4
schemes:
- description: Application ID
  in: header
  name: AppAuth
  parameter: X-App-Id
  sources:
  - openapi/tradera-openapi.json
  type: apiKey
- description: Application Key
  in: header
  name: AppKeyAuth
  parameter: X-App-Key
  sources:
  - openapi/tradera-openapi.json
  type: apiKey
- description: User ID
  in: header
  name: UserAuth
  parameter: X-User-Id
  sources:
  - openapi/tradera-openapi.json
  type: apiKey
- description: User Token
  in: header
  name: UserTokenAuth
  parameter: X-User-Token
  sources:
  - openapi/tradera-openapi.json
  type: apiKey
slug: tradera-authentication
source_filename: tradera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: derived\nsource: openapi/tradera-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AppAuth\n  type: apiKey\n  in: header\n  parameter: X-App-Id\n  description: Application ID\n  sources:\n  - openapi/tradera-openapi.json\n- name: AppKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-App-Key\n  description: Application Key\n  sources:\n  - openapi/tradera-openapi.json\n- name: UserAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Id\n  description: User ID\n  sources:\n  - openapi/tradera-openapi.json\n- name: UserTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Token\n  description: User Token\n  sources:\n  - openapi/tradera-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/authentication/tradera-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Marketplace
- E-Commerce
- Secondhand
- Auctions
- Sweden
---
