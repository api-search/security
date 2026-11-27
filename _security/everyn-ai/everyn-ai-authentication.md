---
anonymous_access: false
api_key_in: []
api_specs:
- filename: everyn-ai-alert-rules-api-openapi.yml
  format: yaml
  label: Everyn Alert Rules API
  slug: everyn-ai-alert-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-alert-rules-api-openapi.yml
- filename: everyn-ai-billing-api-openapi.yml
  format: yaml
  label: Everyn Billing API
  slug: everyn-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-billing-api-openapi.yml
- filename: everyn-ai-callable-jobs-api-openapi.yml
  format: yaml
  label: Everyn Callable Jobs API
  slug: everyn-ai-callable-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-callable-jobs-api-openapi.yml
- filename: everyn-ai-dataset-uploads-api-openapi.yml
  format: yaml
  label: Everyn Dataset Uploads API
  slug: everyn-ai-dataset-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-dataset-uploads-api-openapi.yml
- filename: everyn-ai-datasets-api-openapi.yml
  format: yaml
  label: Everyn Datasets API
  slug: everyn-ai-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-datasets-api-openapi.yml
- filename: everyn-ai-exports-api-openapi.yml
  format: yaml
  label: Everyn Exports API
  slug: everyn-ai-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-exports-api-openapi.yml
- filename: everyn-ai-health-api-openapi.yml
  format: yaml
  label: Everyn Health API
  slug: everyn-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-health-api-openapi.yml
- filename: everyn-ai-job-specs-api-openapi.yml
  format: yaml
  label: Everyn Job Specs API
  slug: everyn-ai-job-specs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-job-specs-api-openapi.yml
- filename: everyn-ai-models-api-openapi.yml
  format: yaml
  label: Everyn Models API
  slug: everyn-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-models-api-openapi.yml
- filename: everyn-ai-organization-admin-api-openapi.yml
  format: yaml
  label: Everyn Organization Admin API
  slug: everyn-ai-organization-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-organization-admin-api-openapi.yml
- filename: everyn-ai-runs-api-openapi.yml
  format: yaml
  label: Everyn Runs API
  slug: everyn-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-runs-api-openapi.yml
- filename: everyn-ai-usage-api-openapi.yml
  format: yaml
  label: Everyn Usage API
  slug: everyn-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-usage-api-openapi.yml
- filename: everyn-ai-webhooks-api-openapi.yml
  format: yaml
  label: Everyn Webhooks API
  slug: everyn-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everyn-ai/openapi/everyn-ai-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Everyn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everyn declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Everyn
provider_slug: everyn-ai
scheme_count: 3
schemes:
- description: 'API key product calls use Authorization: Bearer sk-everyn-...'
  id: BearerAuth
  name: Authorization
  scheme: bearer
  type: http
- description: csrfToken returned by GET /v1/auth/session for the same authenticated browser session.
  id: BrowserCsrf
  in: header
  name: X-CSRF-Token
  type: apiKey
- description: HttpOnly session cookie issued by browser login; deployment may configure its name.
  id: BrowserSession
  in: cookie
  name: everyn_session
  type: apiKey
slug: everyn-ai-authentication
source_filename: everyn-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: authentication.md\nschemes:\n  - type: http\n    scheme: bearer\n    name: Authorization\n    description: \"API key product calls use Authorization: Bearer sk-everyn-...\"\n    id: BearerAuth\n  - type: apiKey\n    in: header\n    name: X-CSRF-Token\n    description: \"csrfToken returned by GET /v1/auth/session for the same authenticated browser session.\"\n    id: BrowserCsrf\n  - type: apiKey\n    in: cookie\n    name: everyn_session\n    description: \"HttpOnly session cookie issued by browser login; deployment may configure its name.\"\n    id: BrowserSession\n"
source_yaml_url: https://artifacts.apis.io/everyn-ai/authentication/everyn-ai-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Automation
- Productivity
- Agents
- Platform
---
