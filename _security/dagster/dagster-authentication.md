---
api_key_in:
- header
api_specs:
- filename: dagster-external-assets-rest-api-openapi.yml
  format: yaml
  label: Dagster External Assets REST API
  slug: external-assets-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagster/refs/heads/main/openapi/dagster-external-assets-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dagster Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dagster secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dagster
provider_slug: dagster
scheme_count: 1
schemes:
- description: User token used to authenticate against Dagster+ deployments.
  in: header
  name: DagsterCloudToken
  parameter: Dagster-Cloud-Api-Token
  sources:
  - openapi/dagster-external-assets-rest-api-openapi.yml
  type: apiKey
slug: dagster-authentication
source_filename: dagster-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dagster-external-assets-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: DagsterCloudToken\n  type: apiKey\n  in: header\n  parameter: Dagster-Cloud-Api-Token\n  description: User token used to authenticate against Dagster+ deployments.\n  sources:\n  - openapi/dagster-external-assets-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagster/refs/heads/main/authentication/dagster-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Engineering
- Data Orchestration
- Data Pipelines
- ETL
- Workflows
- Assets
- GraphQL
---
