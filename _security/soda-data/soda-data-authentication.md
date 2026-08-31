---
api_key_in:
- cookie
api_specs:
- filename: soda-data-cloud-api-v4-openapi.yml
  format: yaml
  label: Soda Cloud API v4
  slug: soda-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/_original/soda-data-cloud-api-v4-openapi.yml
- filename: soda-data-attributes-api-openapi.yml
  format: yaml
  label: Soda Attributes API
  slug: soda-data-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-attributes-api-openapi.yml
- filename: soda-data-checks-api-openapi.yml
  format: yaml
  label: Soda Checks API
  slug: soda-data-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-checks-api-openapi.yml
- filename: soda-data-contracts-api-openapi.yml
  format: yaml
  label: Soda Contracts API
  slug: soda-data-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-contracts-api-openapi.yml
- filename: soda-data-data-standards-api-openapi.yml
  format: yaml
  label: Soda Data Standards API
  slug: soda-data-data-standards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-data-standards-api-openapi.yml
- filename: soda-data-datasets-api-openapi.yml
  format: yaml
  label: Soda Datasets API
  slug: soda-data-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-datasets-api-openapi.yml
- filename: soda-data-datasources-api-openapi.yml
  format: yaml
  label: Soda Datasources API
  slug: soda-data-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-datasources-api-openapi.yml
- filename: soda-data-discovered-datasets-api-openapi.yml
  format: yaml
  label: Soda Discovered Datasets API
  slug: soda-data-discovered-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-discovered-datasets-api-openapi.yml
- filename: soda-data-incidents-api-openapi.yml
  format: yaml
  label: Soda Incidents API
  slug: soda-data-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-incidents-api-openapi.yml
- filename: soda-data-licensing-api-openapi.yml
  format: yaml
  label: Soda Licensing API
  slug: soda-data-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-licensing-api-openapi.yml
- filename: soda-data-notification-rules-api-openapi.yml
  format: yaml
  label: Soda Notification Rules API
  slug: soda-data-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-notification-rules-api-openapi.yml
- filename: soda-data-runners-api-openapi.yml
  format: yaml
  label: Soda Runners API
  slug: soda-data-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-runners-api-openapi.yml
- filename: soda-data-scans-api-openapi.yml
  format: yaml
  label: Soda Scans API
  slug: soda-data-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-scans-api-openapi.yml
- filename: soda-data-secrets-api-openapi.yml
  format: yaml
  label: Soda Secrets API
  slug: soda-data-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-secrets-api-openapi.yml
- filename: soda-data-users-api-openapi.yml
  format: yaml
  label: Soda Users API
  slug: soda-data-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-users-api-openapi.yml
- filename: soda-data-utility-api-openapi.yml
  format: yaml
  label: Soda Utility API
  slug: soda-data-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-utility-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Soda Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soda secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Soda
provider_slug: soda-data
scheme_count: 2
schemes:
- name: basicAuthApiKey
  scheme: basic
  sources:
  - openapi/soda-data-attributes-api-openapi.yml
  - openapi/soda-data-checks-api-openapi.yml
  - openapi/soda-data-contracts-api-openapi.yml
  - openapi/soda-data-data-standards-api-openapi.yml
  - openapi/soda-data-datasets-api-openapi.yml
  - openapi/soda-data-datasources-api-openapi.yml
  - openapi/soda-data-discovered-datasets-api-openapi.yml
  - openapi/soda-data-incidents-api-openapi.yml
  - openapi/soda-data-licensing-api-openapi.yml
  - openapi/soda-data-notification-rules-api-openapi.yml
  - openapi/soda-data-runners-api-openapi.yml
  - openapi/soda-data-scans-api-openapi.yml
  - openapi/soda-data-secrets-api-openapi.yml
  - openapi/soda-data-users-api-openapi.yml
  - openapi/soda-data-utility-api-openapi.yml
  type: http
- in: cookie
  name: cookieToken
  parameter: token
  sources:
  - openapi/soda-data-attributes-api-openapi.yml
  - openapi/soda-data-checks-api-openapi.yml
  - openapi/soda-data-contracts-api-openapi.yml
  - openapi/soda-data-data-standards-api-openapi.yml
  - openapi/soda-data-datasets-api-openapi.yml
  - openapi/soda-data-datasources-api-openapi.yml
  - openapi/soda-data-discovered-datasets-api-openapi.yml
  - openapi/soda-data-incidents-api-openapi.yml
  - openapi/soda-data-licensing-api-openapi.yml
  - openapi/soda-data-notification-rules-api-openapi.yml
  - openapi/soda-data-runners-api-openapi.yml
  - openapi/soda-data-scans-api-openapi.yml
  - openapi/soda-data-secrets-api-openapi.yml
  - openapi/soda-data-users-api-openapi.yml
  - openapi/soda-data-utility-api-openapi.yml
  type: apiKey
slug: soda-data-authentication
source_filename: soda-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/soda-data-attributes-api-openapi.yml, openapi/soda-data-checks-api-openapi.yml,\n  openapi/soda-data-contracts-api-openapi.yml, openapi/soda-data-data-standards-api-openapi.yml,\n  openapi/soda-data-datasets-api-openapi.yml, openapi/soda-data-datasources-api-openapi.yml,\n  openapi/soda-data-discovered-datasets-api-openapi.yml, openapi/soda-data-incidents-api-openapi.yml,\n  openapi/soda-data-licensing-api-openapi.yml, openapi/soda-data-notification-rules-api-openapi.yml,\n  openapi/soda-data-runners-api-openapi.yml, openapi/soda-data-scans-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuthApiKey\n  type: http\n  scheme: basic\n  sources:\n  - openapi/soda-data-attributes-api-openapi.yml\n  - openapi/soda-data-checks-api-openapi.yml\n  - openapi/soda-data-contracts-api-openapi.yml\n  - openapi/soda-data-data-standards-api-openapi.yml\n  - openapi/soda-data-datasets-api-openapi.yml\n\
  \  - openapi/soda-data-datasources-api-openapi.yml\n  - openapi/soda-data-discovered-datasets-api-openapi.yml\n  - openapi/soda-data-incidents-api-openapi.yml\n  - openapi/soda-data-licensing-api-openapi.yml\n  - openapi/soda-data-notification-rules-api-openapi.yml\n  - openapi/soda-data-runners-api-openapi.yml\n  - openapi/soda-data-scans-api-openapi.yml\n  - openapi/soda-data-secrets-api-openapi.yml\n  - openapi/soda-data-users-api-openapi.yml\n  - openapi/soda-data-utility-api-openapi.yml\n- name: cookieToken\n  type: apiKey\n  in: cookie\n  parameter: token\n  sources:\n  - openapi/soda-data-attributes-api-openapi.yml\n  - openapi/soda-data-checks-api-openapi.yml\n  - openapi/soda-data-contracts-api-openapi.yml\n  - openapi/soda-data-data-standards-api-openapi.yml\n  - openapi/soda-data-datasets-api-openapi.yml\n  - openapi/soda-data-datasources-api-openapi.yml\n  - openapi/soda-data-discovered-datasets-api-openapi.yml\n  - openapi/soda-data-incidents-api-openapi.yml\n  - openapi/soda-data-licensing-api-openapi.yml\n\
  \  - openapi/soda-data-notification-rules-api-openapi.yml\n  - openapi/soda-data-runners-api-openapi.yml\n  - openapi/soda-data-scans-api-openapi.yml\n  - openapi/soda-data-secrets-api-openapi.yml\n  - openapi/soda-data-users-api-openapi.yml\n  - openapi/soda-data-utility-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/authentication/soda-data-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AIOps
- Data Quality
- Data Observability
- Data Contracts
- Data Governance
- Anomaly Detection
- Data Monitoring
- Data Testing
---
