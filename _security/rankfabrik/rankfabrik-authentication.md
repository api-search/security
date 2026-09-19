---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Rankfabrik Authentication
name_suffix: Authentication
oauth_flows: []
overview: RankFabrik declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: RankFabrik
provider_slug: rankfabrik
scheme_count: 1
schemes:
- description: Product-scoped secret API key issued at signup (free trial key delivered immediately, no card). Presented on every request in the x-cle-api header.
  id: api_key
  in: header
  key_prefix: rf_
  name: x-cle-api
  scope: per-product (key is bound to one of Places/Jobs/Captions/Verify)
  type: apiKey
slug: rankfabrik-authentication
source_filename: rankfabrik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://rankfabrik.com/documentation\nnote: >-\n  Derived by hand from the developer documentation because RankFabrik publishes no\n  machine-readable OpenAPI (specs are provided on request by email / via Apify\n  marketplaces). All four products use a single scheme: a product-scoped API key\n  passed in the x-cle-api request header. Keys are prefixed rf_ and are not\n  interchangeable across products (a Places key cannot call Jobs). A missing or\n  unknown key returns 401. Verified live: an unauthenticated GET returns\n  HTTP 401 with body {\"error\":\"clé absente — la présenter dans l'en-tête x-cle-api\"}.\ndocs: https://rankfabrik.com/documentation\nschemes:\n  - id: api_key\n    type: apiKey\n    in: header\n    name: x-cle-api\n    key_prefix: rf_\n    scope: per-product (key is bound to one of Places/Jobs/Captions/Verify)\n    description: >-\n      Product-scoped secret API key issued at signup (free trial key delivered\n\
  \      immediately, no card). Presented on every request in the x-cle-api header.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nfailure:\n  status: 401\n  envelope: '{\"error\": \"<message>\"}'\n  observed: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rankfabrik/refs/heads/main/authentication/rankfabrik-authentication.yml
summary_line: 1 scheme
tags:
- Data
- Web Scraping
- Local Business
- Places
- Job
- Job Postings
- video-transcripts
- Captions
- Email Verification
- Data Enrichment
- Lead Generation
- REST API
---
