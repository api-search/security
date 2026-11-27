---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ablakarajanlat-hu-agent-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Agent API
  slug: ablakarajanlat-hu-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-agent-api-openapi.yml
- filename: ablakarajanlat-hu-ai-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat AI API
  slug: ablakarajanlat-hu-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-ai-api-openapi.yml
- filename: ablakarajanlat-hu-coverage-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Coverage API
  slug: ablakarajanlat-hu-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-coverage-api-openapi.yml
- filename: ablakarajanlat-hu-estimate-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Estimate API
  slug: ablakarajanlat-hu-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-estimate-api-openapi.yml
- filename: ablakarajanlat-hu-knowledge-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Knowledge API
  slug: ablakarajanlat-hu-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-knowledge-api-openapi.yml
- filename: ablakarajanlat-hu-mcp-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat MCP API
  slug: ablakarajanlat-hu-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-mcp-api-openapi.yml
- filename: ablakarajanlat-hu-quote-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Quote API
  slug: ablakarajanlat-hu-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-quote-api-openapi.yml
- filename: ablakarajanlat-hu-support-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Support API
  slug: ablakarajanlat-hu-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-support-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ablak Árajánlat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ablak Árajánlat secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ablak Árajánlat
provider_slug: ablakarajanlat-hu
scheme_count: 1
schemes:
- description: 'Opcionális partner/API kulcs.

    Kulcs nélkül publikus limit (1/60mp/IP), kulccsal partner kvóta érvényes.'
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/ablakarajanlat-hu-openapi.yaml
  type: apiKey
slug: ablakarajanlat-hu-authentication
source_filename: ablakarajanlat-hu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/ablakarajanlat-hu-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    Opcionális partner/API kulcs.\n    Kulcs nélkül publikus limit (1/60mp/IP), kulccsal partner kvóta érvényes.\n  sources:\n  - openapi/ablakarajanlat-hu-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/ablakarajanlat-hu/authentication/ablakarajanlat-hu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Windows
- Calculator
- Construction
- Hungary
- Pricing
---
