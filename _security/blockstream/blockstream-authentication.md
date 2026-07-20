---
api_key_in: []
api_specs:
- filename: blockstream-esplora-openapi.yml
  format: yaml
  label: Blockstream Esplora HTTP API
  slug: blockstream-esplora-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-esplora-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Blockstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blockstream declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Blockstream
provider_slug: blockstream
scheme_count: 0
schemes: []
slug: blockstream-authentication
source_filename: blockstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/Blockstream/esplora/blob/master/API.md\ndocs: https://github.com/Blockstream/esplora/blob/master/API.md\nsummary:\n  types: []\n  authentication_required: false\n  note: >-\n    The Blockstream Esplora HTTP API is a public, read-mostly block explorer API\n    that requires no authentication, API key, or OAuth token. All endpoints are\n    open. The single write path (POST /tx broadcast) is also unauthenticated;\n    network consensus rules validate the submitted transaction. There are no\n    securitySchemes declared in the OpenAPI because none are used.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/authentication/blockstream-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Bitcoin
- Blockchain
- Cryptocurrency
- Block Explorer
- Financial Services
- Infrastructure
---
