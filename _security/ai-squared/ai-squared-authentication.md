---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ai-squared-catalogs-api-openapi.yml
  format: yaml
  label: AI Squared Catalogs API
  slug: ai-squared-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-catalogs-api-openapi.yml
- filename: ai-squared-connector-definitions-api-openapi.yml
  format: yaml
  label: AI Squared Connector Definitions API
  slug: ai-squared-connector-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-connector-definitions-api-openapi.yml
- filename: ai-squared-connectors-api-openapi.yml
  format: yaml
  label: AI Squared Connectors API
  slug: ai-squared-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-connectors-api-openapi.yml
- filename: ai-squared-models-api-openapi.yml
  format: yaml
  label: AI Squared Models API
  slug: ai-squared-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-models-api-openapi.yml
- filename: ai-squared-syncrecords-api-openapi.yml
  format: yaml
  label: AI Squared Sync Records API
  slug: ai-squared-syncrecords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncrecords-api-openapi.yml
- filename: ai-squared-syncrun-api-openapi.yml
  format: yaml
  label: AI Squared Sync Run API
  slug: ai-squared-syncrun-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncrun-api-openapi.yml
- filename: ai-squared-syncruns-api-openapi.yml
  format: yaml
  label: AI Squared Sync Runs API
  slug: ai-squared-syncruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncruns-api-openapi.yml
- filename: ai-squared-syncs-api-openapi.yml
  format: yaml
  label: AI Squared Syncs API
  slug: ai-squared-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ai Squared Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Squared secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AI Squared
provider_slug: ai-squared
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ai-squared-openapi.yml
  type: http
slug: ai-squared-authentication
source_filename: ai-squared-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: derived\nsource: openapi/ai-squared-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ai-squared-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/authentication/ai-squared-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Integration
- Reverse ETL
- Artificial Intelligence
- Machine Learning
- Customer Data Platform
- Data Activation
- Workflow Automation
- Open Source
- MCP
- Enterprise
- A2A
---
