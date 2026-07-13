---
api_key_in:
- header
api_specs:
- filename: coresignal-multi-source-company-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Company API
  slug: multi-source-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-company-api-openapi.yml
- filename: coresignal-multi-source-employee-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Employee API
  slug: multi-source-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-employee-api-openapi.yml
- filename: coresignal-multi-source-jobs-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Jobs API
  slug: multi-source-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-jobs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coresignal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coresignal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coresignal
provider_slug: coresignal
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: apikey
  sources:
  - openapi/coresignal-multi-source-company-api-openapi.yml
  - openapi/coresignal-multi-source-employee-api-openapi.yml
  - openapi/coresignal-multi-source-jobs-api-openapi.yml
  type: apiKey
slug: coresignal-authentication
source_filename: coresignal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coresignal-multi-source-company-api-openapi.yml, openapi/coresignal-multi-source-employee-api-openapi.yml,\n  openapi/coresignal-multi-source-jobs-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/coresignal-multi-source-company-api-openapi.yml\n  - openapi/coresignal-multi-source-employee-api-openapi.yml\n  - openapi/coresignal-multi-source-jobs-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/authentication/coresignal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agentic Search
- B2B Data
- Companies
- Company Data
- Data as a Service
- Elasticsearch
- Employee Data
- Employees
- Enrichment
- Firmographics
- Job Postings
- Jobs
- Lead Generation
- People Data
- Sales Intelligence
- Talent Intelligence
- Web Data
---
