---
anonymous_access: false
api_key_in: []
api_specs:
- filename: markmesh-com-clients-api-openapi.yml
  format: yaml
  label: MarkMesh Clients API
  slug: markmesh-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-clients-api-openapi.yml
- filename: markmesh-com-filing-watches-api-openapi.yml
  format: yaml
  label: MarkMesh Filing watches API
  slug: markmesh-com-filing-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-filing-watches-api-openapi.yml
- filename: markmesh-com-filings-api-openapi.yml
  format: yaml
  label: MarkMesh Filings API
  slug: markmesh-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-filings-api-openapi.yml
- filename: markmesh-com-membership-api-openapi.yml
  format: yaml
  label: MarkMesh Membership API
  slug: markmesh-com-membership-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-membership-api-openapi.yml
- filename: markmesh-com-organisation-api-openapi.yml
  format: yaml
  label: MarkMesh Organisation API
  slug: markmesh-com-organisation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-organisation-api-openapi.yml
- filename: markmesh-com-other-api-openapi.yml
  format: yaml
  label: MarkMesh Other API
  slug: markmesh-com-other-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-other-api-openapi.yml
- filename: markmesh-com-partner-api-openapi.yml
  format: yaml
  label: MarkMesh Partner API
  slug: markmesh-com-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-partner-api-openapi.yml
- filename: markmesh-com-reference-api-openapi.yml
  format: yaml
  label: MarkMesh Reference API
  slug: markmesh-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-reference-api-openapi.yml
- filename: markmesh-com-search-api-openapi.yml
  format: yaml
  label: MarkMesh Search API
  slug: markmesh-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-search-api-openapi.yml
- filename: markmesh-com-system-api-openapi.yml
  format: yaml
  label: MarkMesh System API
  slug: markmesh-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-system-api-openapi.yml
- filename: markmesh-com-trademarks-api-openapi.yml
  format: yaml
  label: MarkMesh Trademarks API
  slug: markmesh-com-trademarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markmesh-com/openapi/markmesh-com-trademarks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MarkMesh Authentication
name_suffix: Authentication
oauth_flows: []
overview: MarkMesh secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MarkMesh
provider_slug: markmesh-com
scheme_count: 1
schemes:
- bearerFormat: Opaque API key (prefix mm_live_ or mm_test_)
  description: Static API key for machine integrations. Issued via the UI at `/account/api-keys`. Prefix `mm_live_*` for production, `mm_test_*` for sandbox. Tokens are shown ONCE at creation — store them immediately.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/markmesh-com-openapi.json
  type: http
slug: markmesh-com-authentication
source_filename: markmesh-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/markmesh-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: Opaque API key (prefix mm_live_ or mm_test_)\n  description: Static API key for machine integrations. Issued via the UI at `/account/api-keys`.\n    Prefix `mm_live_*` for production, `mm_test_*` for sandbox. Tokens are shown ONCE at creation\n    — store them immediately.\n  sources:\n  - openapi/markmesh-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/markmesh-com/authentication/markmesh-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Trademark Search
- Portfolio Monitoring
- Law Firm Tools
---
