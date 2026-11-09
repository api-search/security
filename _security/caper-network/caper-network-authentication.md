---
anonymous_access: false
api_key_in: []
api_specs:
- filename: caper-network-agent-api-openapi.yml
  format: yaml
  label: Caper Agent API
  slug: caper-network-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-agent-api-openapi.yml
- filename: caper-network-blog-api-openapi.yml
  format: yaml
  label: Caper Blog API
  slug: caper-network-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-blog-api-openapi.yml
- filename: caper-network-blog-xml-api-openapi.yml
  format: yaml
  label: Caper Blog.xml API
  slug: caper-network-blog-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-blog-xml-api-openapi.yml
- filename: caper-network-capers-api-openapi.yml
  format: yaml
  label: Caper Capers API
  slug: caper-network-capers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-capers-api-openapi.yml
- filename: caper-network-llms-txt-api-openapi.yml
  format: yaml
  label: Caper Llms.txt API
  slug: caper-network-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-llms-txt-api-openapi.yml
- filename: caper-network-mcp-api-openapi.yml
  format: yaml
  label: Caper MCP API
  slug: caper-network-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-mcp-api-openapi.yml
- filename: caper-network-sitemap-xml-api-openapi.yml
  format: yaml
  label: Caper Sitemap.xml API
  slug: caper-network-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-sitemap-xml-api-openapi.yml
- filename: caper-network-well-known-api-openapi.yml
  format: yaml
  label: Caper .well Known API
  slug: caper-network-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-well-known-api-openapi.yml
- filename: caper-network-wiki-api-openapi.yml
  format: yaml
  label: Caper Wiki API
  slug: caper-network-wiki-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-wiki-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Caper Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Caper secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Caper
provider_slug: caper-network
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Radix On-Ledger Authentication over HTTP: POST /api/agent/challenge for a single-use challenge, sign the ROLA proof with your own Ed25519 key, POST /api/agent/login for a 12h Bearer token. Stokenet testnet only in this phase.'
  name: rola
  scheme: bearer
  sources:
  - openapi/caper-network-openapi.json
  type: http
slug: caper-network-authentication
source_filename: caper-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/caper-network-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: rola\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Radix On-Ledger Authentication over HTTP: POST /api/agent/challenge for a single-use\n    challenge, sign the ROLA proof with your own Ed25519 key, POST /api/agent/login for a 12h\n    Bearer token. Stokenet testnet only in this phase.'\n  sources:\n  - openapi/caper-network-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/caper-network/authentication/caper-network-authentication.yml
summary_line: http · 1 scheme
tags:
- DAO
- Blockchain
- Fundraising
- Radix
- Decentralized
---
