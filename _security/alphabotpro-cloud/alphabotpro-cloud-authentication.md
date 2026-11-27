---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alphabotpro-cloud-checkout-api-openapi.yml
  format: yaml
  label: AlphaBotPro Checkout API
  slug: alphabotpro-cloud-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-checkout-api-openapi.yml
- filename: alphabotpro-cloud-ea-api-openapi.yml
  format: yaml
  label: AlphaBotPro Ea API
  slug: alphabotpro-cloud-ea-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-ea-api-openapi.yml
- filename: alphabotpro-cloud-expert-advisors-api-openapi.yml
  format: yaml
  label: AlphaBotPro Expert Advisors API
  slug: alphabotpro-cloud-expert-advisors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-expert-advisors-api-openapi.yml
- filename: alphabotpro-cloud-mcp-api-openapi.yml
  format: yaml
  label: AlphaBotPro MCP API
  slug: alphabotpro-cloud-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-mcp-api-openapi.yml
- filename: alphabotpro-cloud-signals-api-openapi.yml
  format: yaml
  label: AlphaBotPro Signals API
  slug: alphabotpro-cloud-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-signals-api-openapi.yml
- filename: alphabotpro-cloud-stocks-api-openapi.yml
  format: yaml
  label: AlphaBotPro Stocks API
  slug: alphabotpro-cloud-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-stocks-api-openapi.yml
- filename: alphabotpro-cloud-warroom-api-openapi.yml
  format: yaml
  label: AlphaBotPro Warroom API
  slug: alphabotpro-cloud-warroom-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-warroom-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AlphaBotPro Authentication
name_suffix: Authentication
oauth_flows: []
overview: AlphaBotPro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AlphaBotPro
provider_slug: alphabotpro-cloud
scheme_count: 1
schemes:
- description: API key in the format abp_<env>_<publicId>_<secret>
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alphabotpro-cloud-openapi.json
  - openapi/mcp-alphabotpro-cloud-openapi.json
  type: http
slug: alphabotpro-cloud-authentication
source_filename: alphabotpro-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/alphabotpro-cloud-openapi.json, openapi/mcp-alphabotpro-cloud-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key in the format abp_<env>_<publicId>_<secret>\n  sources:\n  - openapi/alphabotpro-cloud-openapi.json\n  - openapi/mcp-alphabotpro-cloud-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/alphabotpro-cloud/authentication/alphabotpro-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Trading
- Automation
- Signals
- MT5
- PropFirm
---
