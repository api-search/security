---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: paketsoft-com-katalog-api-openapi.yml
  format: yaml
  label: PaketSoft Katalog API
  slug: paketsoft-com-katalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-katalog-api-openapi.yml
- filename: paketsoft-com-kuponlar-api-openapi.yml
  format: yaml
  label: PaketSoft Kuponlar API
  slug: paketsoft-com-kuponlar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-kuponlar-api-openapi.yml
- filename: paketsoft-com-m-teriler-api-openapi.yml
  format: yaml
  label: PaketSoft Müşteriler API
  slug: paketsoft-com-m-teriler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-m-teriler-api-openapi.yml
- filename: paketsoft-com-r-nler-api-openapi.yml
  format: yaml
  label: PaketSoft Ürünler API
  slug: paketsoft-com-r-nler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-r-nler-api-openapi.yml
- filename: paketsoft-com-rapor-api-openapi.yml
  format: yaml
  label: PaketSoft Rapor API
  slug: paketsoft-com-rapor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-rapor-api-openapi.yml
- filename: paketsoft-com-sipari-ler-api-openapi.yml
  format: yaml
  label: PaketSoft Siparişler API
  slug: paketsoft-com-sipari-ler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-sipari-ler-api-openapi.yml
- filename: paketsoft-com-webhooklar-api-openapi.yml
  format: yaml
  label: PaketSoft Webhooklar API
  slug: paketsoft-com-webhooklar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paketsoft-com/openapi/paketsoft-com-webhooklar-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: PaketSoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: PaketSoft secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PaketSoft
provider_slug: paketsoft-com
scheme_count: 3
schemes:
- description: pk_ ile başlayan anahtar
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/paketsoft-com-openapi.json
  type: apiKey
- description: sk_ ile başlayan gizli anahtar
  in: header
  name: apiSecret
  parameter: X-Api-Secret
  sources:
  - openapi/paketsoft-com-openapi.json
  type: apiKey
- description: base64(anahtar:gizli)
  name: basic
  scheme: basic
  sources:
  - openapi/paketsoft-com-openapi.json
  type: http
slug: paketsoft-com-authentication
source_filename: paketsoft-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/paketsoft-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: pk_ ile başlayan anahtar\n  sources:\n  - openapi/paketsoft-com-openapi.json\n- name: apiSecret\n  type: apiKey\n  in: header\n  parameter: X-Api-Secret\n  description: sk_ ile başlayan gizli anahtar\n  sources:\n  - openapi/paketsoft-com-openapi.json\n- name: basic\n  type: http\n  scheme: basic\n  description: base64(anahtar:gizli)\n  sources:\n  - openapi/paketsoft-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/paketsoft-com/authentication/paketsoft-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
---
