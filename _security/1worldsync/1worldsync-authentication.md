---
api_key_in:
- header
- query
api_specs:
- filename: 1worldsync-content1-openapi-original.json
  format: json
  label: 1WorldSync Content1 API
  slug: 1worldsync-content1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1worldsync/refs/heads/main/openapi/1worldsync-content1-openapi-original.json
auth_types:
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: 1Worldsync Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1WorldSync secures its APIs with hmac across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 1WorldSync
provider_slug: 1worldsync
scheme_count: 1
schemes:
- description: Each request is signed by building a canonical string and computing an HMAC-SHA256 hash with the account secret key. The signature (hashcode) proves the sender identity.
  name: HMAC
  parameters:
  - description: 8-character alphanumeric application identifier issued at registration.
    in: header
    name: appid
    required: true
  - description: HMAC signature (hash_code) of the request computed with the secret key.
    in: header
    name: hashcode
    required: true
  - description: UTC timestamp included in the signed string.
    in: query
    name: timestamp
    required: true
  - description: Optional Global Location Number scoping the request.
    in: header
    name: gln
    required: false
  sources:
  - openapi/1worldsync-content1-openapi-original.json
  - https://developer.1worldsync.com/wp-content/uploads/2022/11/1WorldSync_Content1_API_HMAC_Guide.pdf
  type: hmac
slug: 1worldsync-authentication
source_filename: 1worldsync-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developer.1worldsync.com/read-api-2-0-documentation/\ndocs: https://developer.1worldsync.com/wp-content/uploads/2022/11/1WorldSync_Content1_API_HMAC_Guide.pdf\nsummary:\n  types: [hmac]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  note: >-\n    1WorldSync Content1 APIs use HMAC-signed requests. There is no OpenAPI\n    securityScheme declared; authentication is carried in request headers and a\n    query parameter. Credentials (an 8-character alphanumeric app_id and a\n    32-character secret key) are issued at registration; separate credentials are\n    issued for the Pre-Production environment.\nschemes:\n- name: HMAC\n  type: hmac\n  description: >-\n    Each request is signed by building a canonical string and computing an\n    HMAC-SHA256 hash with the account secret key. The signature (hashcode) proves\n    the sender identity.\n  parameters:\n  - name: appid\n    in: header\n    required: true\n    description:\
  \ 8-character alphanumeric application identifier issued at registration.\n  - name: hashcode\n    in: header\n    required: true\n    description: HMAC signature (hash_code) of the request computed with the secret key.\n  - name: timestamp\n    in: query\n    required: true\n    description: UTC timestamp included in the signed string.\n  - name: gln\n    in: header\n    required: false\n    description: Optional Global Location Number scoping the request.\n  sources:\n  - openapi/1worldsync-content1-openapi-original.json\n  - https://developer.1worldsync.com/wp-content/uploads/2022/11/1WorldSync_Content1_API_HMAC_Guide.pdf\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1worldsync/refs/heads/main/authentication/1worldsync-authentication.yml
summary_line: hmac · 1 scheme
tags:
- Company
- Product Content
- GDSN
- Data Syndication
- Master Data
- Digital Shelf
- Product Information Management
- PIM
- CPG
- Retail
- GS1
---
