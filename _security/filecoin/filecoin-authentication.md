---
api_key_in: []
api_specs:
- filename: filecoin-http-api
  format: yaml
  label: Filecoin HTTP REST API
  slug: filecoin-http-rest-api
  spec_type: OpenAPI
  url: https://github.com/filecoin-project/filecoin-http-api
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Filecoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filecoin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Filecoin
provider_slug: filecoin
scheme_count: 1
schemes:
- description: 'The authentication scheme for this API is implementation dependent. Implementations should feel free to use the scheme and granularity they deem fit. This document describes the scheme used by the [go-filecoin](https://github.com/filecoin-project/go-filecoin) daemon.


    Go-filecoin will initially (v0) support a simple all or nothing authentication and authorization suitable for use by the owner/oper'
  name: BearerTokenAuth
  scheme: Bearer Token
  sources:
  - openapi/api.yml
  type: http
slug: filecoin-authentication
source_filename: filecoin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerTokenAuth\n  type: http\n  scheme: Bearer Token\n  description: |-\n    The authentication scheme for this API is implementation dependent. Implementations should feel free to use the scheme and granularity they deem fit. This document describes the scheme used by the [go-filecoin](https://github.com/filecoin-project/go-filecoin) daemon.\n\n    Go-filecoin will initially (v0) support a simple all or nothing authentication and authorization suitable for use by the owner/oper\n  sources:\n  - openapi/api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filecoin/refs/heads/main/authentication/filecoin-authentication.yml
summary_line: http · 1 scheme
tags:
- Decentralized Storage
- Web3
- IPFS
- Blockchain
- Storage Deals
- Filecoin+
- FVM
---
