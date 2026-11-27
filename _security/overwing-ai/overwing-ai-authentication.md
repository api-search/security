---
anonymous_access: false
api_key_in: []
api_specs:
- filename: overwing-ai-account-api-openapi.yml
  format: yaml
  label: Overwing Account API
  slug: overwing-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-account-api-openapi.yml
- filename: overwing-ai-atlas-api-openapi.yml
  format: yaml
  label: Overwing Atlas API
  slug: overwing-ai-atlas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-atlas-api-openapi.yml
- filename: overwing-ai-beacon-api-openapi.yml
  format: yaml
  label: Overwing Beacon API
  slug: overwing-ai-beacon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-beacon-api-openapi.yml
- filename: overwing-ai-billing-api-openapi.yml
  format: yaml
  label: Overwing Billing API
  slug: overwing-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-billing-api-openapi.yml
- filename: overwing-ai-cad-api-openapi.yml
  format: yaml
  label: Overwing CAD API
  slug: overwing-ai-cad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-cad-api-openapi.yml
- filename: overwing-ai-evaluate-api-openapi.yml
  format: yaml
  label: Overwing Evaluate API
  slug: overwing-ai-evaluate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-evaluate-api-openapi.yml
- filename: overwing-ai-meta-api-openapi.yml
  format: yaml
  label: Overwing Meta API
  slug: overwing-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-meta-api-openapi.yml
- filename: overwing-ai-onboarding-api-openapi.yml
  format: yaml
  label: Overwing Onboarding API
  slug: overwing-ai-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-onboarding-api-openapi.yml
- filename: overwing-ai-preflight-api-openapi.yml
  format: yaml
  label: Overwing Preflight API
  slug: overwing-ai-preflight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-preflight-api-openapi.yml
- filename: overwing-ai-rule-sets-api-openapi.yml
  format: yaml
  label: Overwing Rule sets API
  slug: overwing-ai-rule-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-rule-sets-api-openapi.yml
- filename: overwing-ai-tower-api-openapi.yml
  format: yaml
  label: Overwing Tower API
  slug: overwing-ai-tower-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/overwing-ai/openapi/overwing-ai-tower-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Overwing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Overwing secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Overwing
provider_slug: overwing-ai
scheme_count: 1
schemes:
- bearerFormat: ow_live_<32 hex>
  description: 'API key from the dashboard, from POST /api/v1/api-keys, or from POST /api/v1/signup (one call, no browser). A key has a scope: full (every endpoint) or evaluate (POST evaluate and evaluate/batch, GET rule-sets, me, usage and the Atlas reads; everything else answers 403). Give agents an evaluate key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/overwing-ai-openapi.json
  type: http
slug: overwing-ai-authentication
source_filename: overwing-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/overwing-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ow_live_<32 hex>\n  description: 'API key from the dashboard, from POST /api/v1/api-keys, or from POST /api/v1/signup\n    (one call, no browser). A key has a scope: full (every endpoint) or evaluate (POST evaluate\n    and evaluate/batch, GET rule-sets, me, usage and the Atlas reads; everything else answers\n    403). Give agents an evaluate key.'\n  sources:\n  - openapi/overwing-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/overwing-ai/authentication/overwing-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Agents
- Guardrails
- Legacy Systems
- IBM
- SAP
---
