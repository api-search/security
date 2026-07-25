---
api_key_in:
- query
api_specs:
- filename: figure-eight-account-info-api-openapi.yml
  format: yaml
  label: Figure Eight Account Info API
  slug: figure-eight-account-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-account-info-api-openapi.yml
- filename: figure-eight-job-create-update-api-openapi.yml
  format: yaml
  label: Figure Eight Job Create/Update API
  slug: figure-eight-job-create-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-job-create-update-api-openapi.yml
- filename: figure-eight-job-ontology-api-openapi.yml
  format: yaml
  label: Figure Eight Job Ontology API
  slug: figure-eight-job-ontology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-job-ontology-api-openapi.yml
- filename: figure-eight-job-results-api-openapi.yml
  format: yaml
  label: Figure Eight Job Results API
  slug: figure-eight-job-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-job-results-api-openapi.yml
- filename: figure-eight-job-status-api-openapi.yml
  format: yaml
  label: Figure Eight Job Status API
  slug: figure-eight-job-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-job-status-api-openapi.yml
- filename: figure-eight-manage-job-data-api-openapi.yml
  format: yaml
  label: Figure Eight Manage Job Data API
  slug: figure-eight-manage-job-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-manage-job-data-api-openapi.yml
- filename: figure-eight-manage-job-settings-api-openapi.yml
  format: yaml
  label: Figure Eight Manage Job Settings API
  slug: figure-eight-manage-job-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-manage-job-settings-api-openapi.yml
- filename: figure-eight-monitor-contributors-api-openapi.yml
  format: yaml
  label: Figure Eight Monitor Contributors API
  slug: figure-eight-monitor-contributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-monitor-contributors-api-openapi.yml
- filename: figure-eight-workflow-data-upload-download-api-openapi.yml
  format: yaml
  label: Figure Eight Workflow Data Upload/Download API
  slug: figure-eight-workflow-data-upload-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflow-data-upload-download-api-openapi.yml
- filename: figure-eight-workflow-filter-rules-api-openapi.yml
  format: yaml
  label: Figure Eight Workflow Filter Rules API
  slug: figure-eight-workflow-filter-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflow-filter-rules-api-openapi.yml
- filename: figure-eight-workflow-step-routes-api-openapi.yml
  format: yaml
  label: Figure Eight Workflow Step Routes API
  slug: figure-eight-workflow-step-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflow-step-routes-api-openapi.yml
- filename: figure-eight-workflow-steps-api-openapi.yml
  format: yaml
  label: Figure Eight Workflow Steps API
  slug: figure-eight-workflow-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflow-steps-api-openapi.yml
- filename: figure-eight-workflows-api-openapi.yml
  format: yaml
  label: Figure Eight Workflows API
  slug: figure-eight-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Figure Eight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Figure Eight secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Figure Eight
provider_slug: figure-eight
scheme_count: 1
schemes:
- description: Account API key passed as the `key` query parameter on every request.
  in: query
  name: apiKey
  parameter: key
  sources:
  - docs
  type: apiKey
slug: figure-eight-authentication
source_filename: figure-eight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://success.figure-eight.com/hc/en-us/articles/201856219-CrowdFlower-API-at-a-Glance\nnote: >-\n  The published OpenAPI declares no components.securitySchemes; the auth model is\n  documented in the API-at-a-Glance guide. Authentication is API-key based: every\n  request must carry a `key` query parameter set to the account API key (found in\n  the platform UI under Account > API). All traffic is over HTTPS.\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Account API key passed as the `key` query parameter on every request.\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/authentication/figure-eight-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Machine Learning
- Data Labeling
- Data Annotation
- Training Data
- Human-in-the-Loop
- Crowdsourcing
- Acquired
---
