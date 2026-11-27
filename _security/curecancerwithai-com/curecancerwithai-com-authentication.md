---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: curecancerwithai-com-blog-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI Blog API
  slug: curecancerwithai-com-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-blog-api-openapi.yml
- filename: curecancerwithai-com-clinical-trials-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI Clinical Trials API
  slug: curecancerwithai-com-clinical-trials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-clinical-trials-api-openapi.yml
- filename: curecancerwithai-com-fda-approvals-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI FDA Approvals API
  slug: curecancerwithai-com-fda-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-fda-approvals-api-openapi.yml
- filename: curecancerwithai-com-inference-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI Inference API
  slug: curecancerwithai-com-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-inference-api-openapi.yml
- filename: curecancerwithai-com-mammal-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI MAMMAL API
  slug: curecancerwithai-com-mammal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-mammal-api-openapi.yml
- filename: curecancerwithai-com-meta-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI Meta API
  slug: curecancerwithai-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-meta-api-openapi.yml
- filename: curecancerwithai-com-news-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI News API
  slug: curecancerwithai-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-news-api-openapi.yml
- filename: curecancerwithai-com-pharma-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI Pharma API
  slug: curecancerwithai-com-pharma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-pharma-api-openapi.yml
- filename: curecancerwithai-com-research-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI Research API
  slug: curecancerwithai-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-research-api-openapi.yml
- filename: curecancerwithai-com-search-api-openapi.yml
  format: yaml
  label: Cure Cancer With AI Search API
  slug: curecancerwithai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curecancerwithai-com/openapi/curecancerwithai-com-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cure Cancer With AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cure Cancer With AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cure Cancer With AI
provider_slug: curecancerwithai-com
scheme_count: 2
schemes:
- description: 'API key as a Bearer token: Authorization: Bearer ccw_live_YOUR_KEY (preferred).'
  name: bearerAuth
  preferred: true
  scheme: bearer
  sources:
  - openapi/curecancerwithai-com-openapi.yml
  - https://www.curecancerwithai.com/ai-api-instructions.md
  type: http
- description: API key in the x-api-key header (alternative to the Bearer token).
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/curecancerwithai-com-openapi.yml
  - https://www.curecancerwithai.com/ai-api-instructions.md
  type: apiKey
slug: curecancerwithai-com-authentication
source_filename: curecancerwithai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.curecancerwithai.com/ai-api-instructions.md\ndocs: https://www.curecancerwithai.com/ai-api-instructions.md\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  key_prefix: ccw_live_\n  key_issuance: 'A user must sign in at https://www.curecancerwithai.com/api-keys and click \"Create key\". The full key (format ccw_live_...) is shown exactly once at creation and cannot be retrieved later.'\n  revocation: Keys can be revoked at any time from the same page.\n  failure: Requests with a missing, invalid, or revoked key return HTTP 401.\n  mcp_auth: 'Remote MCP server at https://www.curecancerwithai.com/api/mcp takes Authorization: Bearer ccw_live_YOUR_KEY.'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  preferred: true\n  description: 'API key as a Bearer token: Authorization: Bearer ccw_live_YOUR_KEY (preferred).'\n  sources:\n  - openapi/curecancerwithai-com-openapi.yml\n  - https://www.curecancerwithai.com/ai-api-instructions.md\n\
  - name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'API key in the x-api-key header (alternative to the Bearer token).'\n  sources:\n  - openapi/curecancerwithai-com-openapi.yml\n  - https://www.curecancerwithai.com/ai-api-instructions.md\n"
source_yaml_url: https://artifacts.apis.io/curecancerwithai-com/authentication/curecancerwithai-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Cancer
- Oncology
- Healthcare
- Clinical Trials
- Biomedical AI
- Medical Research
- MCP
---
