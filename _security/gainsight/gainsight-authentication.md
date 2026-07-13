---
api_key_in:
- header
api_specs:
- filename: gainsight-rest-api-openapi.yml
  format: yaml
  label: Gainsight REST API
  slug: gainsight-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-rest-api-openapi.yml
- filename: gainsight-px-api-openapi.yml
  format: yaml
  label: Gainsight PX API
  slug: gainsight-px-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-px-api-openapi.yml
- filename: gainsight-cs-company-api-openapi.yml
  format: yaml
  label: Gainsight CS Company API
  slug: gainsight-cs-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-company-api-openapi.yml
- filename: gainsight-cs-person-api-openapi.yml
  format: yaml
  label: Gainsight CS Person API
  slug: gainsight-cs-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-person-api-openapi.yml
- filename: gainsight-cs-custom-object-api-openapi.yml
  format: yaml
  label: Gainsight CS Custom Object API
  slug: gainsight-cs-custom-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-custom-object-api-openapi.yml
- filename: gainsight-cs-cta-api-openapi.yml
  format: yaml
  label: Gainsight CS CTA API
  slug: gainsight-cs-cta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-cta-api-openapi.yml
- filename: gainsight-cs-timeline-api-openapi.yml
  format: yaml
  label: Gainsight CS Timeline API
  slug: gainsight-cs-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-timeline-api-openapi.yml
- filename: gainsight-cs-success-plan-api-openapi.yml
  format: yaml
  label: Gainsight CS Success Plan API
  slug: gainsight-cs-success-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-success-plan-api-openapi.yml
- filename: gainsight-cs-data-management-api-openapi.yml
  format: yaml
  label: Gainsight CS Data Management API
  slug: gainsight-cs-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-data-management-api-openapi.yml
- filename: gainsight-cs-bulk-api-openapi.yml
  format: yaml
  label: Gainsight CS Bulk API
  slug: gainsight-cs-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-bulk-api-openapi.yml
- filename: gainsight-cs-events-api-openapi.yml
  format: yaml
  label: Gainsight CS Events API
  slug: gainsight-cs-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-events-api-openapi.yml
- filename: gainsight-cs-user-management-api-openapi.yml
  format: yaml
  label: Gainsight CS User Management API
  slug: gainsight-cs-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-user-management-api-openapi.yml
- filename: gainsight-cs-customer-goals-api-openapi.yml
  format: yaml
  label: Gainsight CS Customer Goals API
  slug: gainsight-cs-customer-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-customer-goals-api-openapi.yml
- filename: gainsight-cs-renewal-center-api-openapi.yml
  format: yaml
  label: Gainsight CS Renewal Center API
  slug: gainsight-cs-renewal-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-renewal-center-api-openapi.yml
- filename: gainsight-cs-task-and-playbook-api-openapi.yml
  format: yaml
  label: Gainsight CS Task and Playbook API
  slug: gainsight-cs-task-and-playbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-task-and-playbook-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gainsight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gainsight secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gainsight
provider_slug: gainsight
scheme_count: 2
schemes:
- description: Gainsight CS REST API access key
  in: header
  name: apiKey
  parameter: accessKey
  sources:
  - openapi/gainsight-cs-bulk-api-openapi.yml
  - openapi/gainsight-cs-company-api-openapi.yml
  - openapi/gainsight-cs-cta-api-openapi.yml
  - openapi/gainsight-cs-custom-object-api-openapi.yml
  - openapi/gainsight-cs-customer-goals-api-openapi.yml
  - openapi/gainsight-cs-data-management-api-openapi.yml
  - openapi/gainsight-cs-events-api-openapi.yml
  - openapi/gainsight-cs-person-api-openapi.yml
  - openapi/gainsight-cs-renewal-center-api-openapi.yml
  - openapi/gainsight-cs-success-plan-api-openapi.yml
  - openapi/gainsight-cs-task-and-playbook-api-openapi.yml
  - openapi/gainsight-cs-timeline-api-openapi.yml
  - openapi/gainsight-cs-user-management-api-openapi.yml
  - openapi/gainsight-rest-api-openapi.yml
  type: apiKey
- description: Gainsight PX API key
  in: header
  name: apiKey
  parameter: X-APTRINSIC-API-KEY
  sources:
  - openapi/gainsight-px-api-openapi.yml
  type: apiKey
slug: gainsight-authentication
source_filename: gainsight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gainsight-cs-bulk-api-openapi.yml, openapi/gainsight-cs-company-api-openapi.yml,\n  openapi/gainsight-cs-cta-api-openapi.yml, openapi/gainsight-cs-custom-object-api-openapi.yml,\n  openapi/gainsight-cs-customer-goals-api-openapi.yml, openapi/gainsight-cs-data-management-api-openapi.yml,\n  openapi/gainsight-cs-events-api-openapi.yml, openapi/gainsight-cs-person-api-openapi.yml,\n  openapi/gainsight-cs-renewal-center-api-openapi.yml, openapi/gainsight-cs-success-plan-api-openapi.yml,\n  openapi/gainsight-cs-task-and-playbook-api-openapi.yml, openapi/gainsight-cs-timeline-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: accessKey\n  description: Gainsight CS REST API access key\n  sources:\n  - openapi/gainsight-cs-bulk-api-openapi.yml\n  - openapi/gainsight-cs-company-api-openapi.yml\n  - openapi/gainsight-cs-cta-api-openapi.yml\n\
  \  - openapi/gainsight-cs-custom-object-api-openapi.yml\n  - openapi/gainsight-cs-customer-goals-api-openapi.yml\n  - openapi/gainsight-cs-data-management-api-openapi.yml\n  - openapi/gainsight-cs-events-api-openapi.yml\n  - openapi/gainsight-cs-person-api-openapi.yml\n  - openapi/gainsight-cs-renewal-center-api-openapi.yml\n  - openapi/gainsight-cs-success-plan-api-openapi.yml\n  - openapi/gainsight-cs-task-and-playbook-api-openapi.yml\n  - openapi/gainsight-cs-timeline-api-openapi.yml\n  - openapi/gainsight-cs-user-management-api-openapi.yml\n  - openapi/gainsight-rest-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-APTRINSIC-API-KEY\n  description: Gainsight PX API key\n  sources:\n  - openapi/gainsight-px-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/authentication/gainsight-authentication.yml
summary_line: apiKey · 2 schemes
tags: []
---
