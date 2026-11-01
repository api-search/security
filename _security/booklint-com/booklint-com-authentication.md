---
anonymous_access: false
api_key_in: []
api_specs:
- filename: booklint-com-booklint-api-openapi.yml
  format: yaml
  label: booklint-com Booklint API
  slug: booklint-com-booklint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-booklint-api-openapi.yml
- filename: booklint-com-check-accounts-tieout-api-openapi.yml
  format: yaml
  label: booklint-com Check Accounts Tieout API
  slug: booklint-com-check-accounts-tieout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-accounts-tieout-api-openapi.yml
- filename: booklint-com-check-api-openapi.yml
  format: yaml
  label: booklint-com Check API
  slug: booklint-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-api-openapi.yml
- filename: booklint-com-check-budget-variance-api-openapi.yml
  format: yaml
  label: booklint-com Check Budget Variance API
  slug: booklint-com-check-budget-variance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-budget-variance-api-openapi.yml
- filename: booklint-com-check-invoice-api-openapi.yml
  format: yaml
  label: booklint-com Check Invoice API
  slug: booklint-com-check-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-invoice-api-openapi.yml
- filename: booklint-com-check-quote-math-api-openapi.yml
  format: yaml
  label: booklint-com Check Quote Math API
  slug: booklint-com-check-quote-math-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-quote-math-api-openapi.yml
- filename: booklint-com-health-api-openapi.yml
  format: yaml
  label: booklint-com Health API
  slug: booklint-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-health-api-openapi.yml
- filename: booklint-com-keys-api-openapi.yml
  format: yaml
  label: booklint-com Keys API
  slug: booklint-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-keys-api-openapi.yml
- filename: booklint-com-llms-txt-api-openapi.yml
  format: yaml
  label: booklint-com Llms.txt API
  slug: booklint-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-llms-txt-api-openapi.yml
- filename: booklint-com-mcp-api-openapi.yml
  format: yaml
  label: booklint-com MCP API
  slug: booklint-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-mcp-api-openapi.yml
- filename: booklint-com-openapi-json-api-openapi.yml
  format: yaml
  label: booklint-com Openapi.json API
  slug: booklint-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-openapi-json-api-openapi.yml
- filename: booklint-com-plans-api-openapi.yml
  format: yaml
  label: booklint-com Plans API
  slug: booklint-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-plans-api-openapi.yml
- filename: booklint-com-privacy-api-openapi.yml
  format: yaml
  label: booklint-com Privacy API
  slug: booklint-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-privacy-api-openapi.yml
- filename: booklint-com-sample-api-openapi.yml
  format: yaml
  label: booklint-com Sample API
  slug: booklint-com-sample-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-sample-api-openapi.yml
- filename: booklint-com-terms-api-openapi.yml
  format: yaml
  label: booklint-com Terms API
  slug: booklint-com-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-terms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Booklint Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: booklint-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: booklint-com
provider_slug: booklint-com
scheme_count: 1
schemes:
- description: A key from POST /v1/keys (vdk_...)
  name: bearer
  scheme: bearer
  sources:
  - openapi/booklint-com-openapi.json
  type: http
slug: booklint-com-authentication
source_filename: booklint-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/booklint-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: A key from POST /v1/keys (vdk_...)\n  sources:\n  - openapi/booklint-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/booklint-com/authentication/booklint-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Spending
- Automation
- API
- Guardrails
- SaaS
---
