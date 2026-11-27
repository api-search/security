---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cryptokeyhole-charts-api-openapi.yml
  format: yaml
  label: CryptoKeyhole Charts API
  slug: cryptokeyhole-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptokeyhole/openapi/cryptokeyhole-charts-api-openapi.yml
- filename: cryptokeyhole-indices-api-openapi.yml
  format: yaml
  label: CryptoKeyhole Indices API
  slug: cryptokeyhole-indices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptokeyhole/openapi/cryptokeyhole-indices-api-openapi.yml
- filename: cryptokeyhole-markets-api-openapi.yml
  format: yaml
  label: CryptoKeyhole Markets API
  slug: cryptokeyhole-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptokeyhole/openapi/cryptokeyhole-markets-api-openapi.yml
- filename: cryptokeyhole-platform-api-openapi.yml
  format: yaml
  label: CryptoKeyhole Platform API
  slug: cryptokeyhole-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptokeyhole/openapi/cryptokeyhole-platform-api-openapi.yml
- filename: cryptokeyhole-tools-api-openapi.yml
  format: yaml
  label: CryptoKeyhole Tools API
  slug: cryptokeyhole-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptokeyhole/openapi/cryptokeyhole-tools-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CryptoKeyhole Authentication
name_suffix: Authentication
oauth_flows: []
overview: CryptoKeyhole declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CryptoKeyhole
provider_slug: cryptokeyhole
scheme_count: 1
schemes:
- description: 'Read-only API key sent as Authorization: Bearer <key>, for Plus and higher plans. The Free view needs no key.'
  name: bearerAuth
  scheme: bearer
  type: http
slug: cryptokeyhole-authentication
source_filename: cryptokeyhole-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://cryptokeyhole.com/api/v1/openapi.json\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Read-only API key sent as Authorization: Bearer <key>, for Plus and\n    higher plans. The Free view needs no key.'\noauth: false\n"
source_yaml_url: https://artifacts.apis.io/cryptokeyhole/authentication/cryptokeyhole-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Blockchain
- Analytics
- Data
- Charts
---
