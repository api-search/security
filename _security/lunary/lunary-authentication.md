---
api_key_in: []
api_specs:
- filename: lunary-analytics-api-openapi.yml
  format: yaml
  label: Lunary Analytics API
  slug: lunary-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-analytics-api-openapi.yml
- filename: lunary-auditlogs-api-openapi.yml
  format: yaml
  label: Lunary AuditLogs API
  slug: lunary-auditlogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-auditlogs-api-openapi.yml
- filename: lunary-checklists-api-openapi.yml
  format: yaml
  label: Lunary Checklists API
  slug: lunary-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-checklists-api-openapi.yml
- filename: lunary-datasets-api-openapi.yml
  format: yaml
  label: Lunary Datasets API
  slug: lunary-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-datasets-api-openapi.yml
- filename: lunary-datasetsv2-api-openapi.yml
  format: yaml
  label: Lunary DatasetsV2 API
  slug: lunary-datasetsv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-datasetsv2-api-openapi.yml
- filename: lunary-evals-api-openapi.yml
  format: yaml
  label: Lunary Evals API
  slug: lunary-evals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-evals-api-openapi.yml
- filename: lunary-externalusers-api-openapi.yml
  format: yaml
  label: Lunary ExternalUsers API
  slug: lunary-externalusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-externalusers-api-openapi.yml
- filename: lunary-models-api-openapi.yml
  format: yaml
  label: Lunary Models API
  slug: lunary-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-models-api-openapi.yml
- filename: lunary-playground-api-openapi.yml
  format: yaml
  label: Lunary Playground API
  slug: lunary-playground-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-playground-api-openapi.yml
- filename: lunary-runs-api-openapi.yml
  format: yaml
  label: Lunary Runs API
  slug: lunary-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-runs-api-openapi.yml
- filename: lunary-templates-api-openapi.yml
  format: yaml
  label: Lunary Templates API
  slug: lunary-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-templates-api-openapi.yml
- filename: lunary-testendpoint-api-openapi.yml
  format: yaml
  label: Lunary TestEndpoint API
  slug: lunary-testendpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-testendpoint-api-openapi.yml
- filename: lunary-views-api-openapi.yml
  format: yaml
  label: Lunary Views API
  slug: lunary-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-views-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lunary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lunary secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lunary
provider_slug: lunary
scheme_count: 1
schemes:
- bearerFormat: Lunary project private API key (UUID)
  name: ProjectPrivateApiKeyAuth
  scheme: bearer
  sources:
  - openapi/lunary-openapi.yml
  type: http
slug: lunary-authentication
source_filename: lunary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lunary-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ProjectPrivateApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Lunary project private API key (UUID)\n  sources:\n  - openapi/lunary-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/authentication/lunary-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Evaluation
- Observability
- Open-Source
- LLM
- Tracing
- Prompts
---
