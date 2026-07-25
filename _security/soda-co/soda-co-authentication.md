---
api_key_in: []
api_specs:
- filename: soda-co-attributes-api-openapi.yml
  format: yaml
  label: Soda Attributes API
  slug: soda-co-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-attributes-api-openapi.yml
- filename: soda-co-checks-api-openapi.yml
  format: yaml
  label: Soda Checks API
  slug: soda-co-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-checks-api-openapi.yml
- filename: soda-co-contracts-api-openapi.yml
  format: yaml
  label: Soda Contracts API
  slug: soda-co-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-contracts-api-openapi.yml
- filename: soda-co-datasets-api-openapi.yml
  format: yaml
  label: Soda Datasets API
  slug: soda-co-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-datasets-api-openapi.yml
- filename: soda-co-datasources-api-openapi.yml
  format: yaml
  label: Soda Datasources API
  slug: soda-co-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-datasources-api-openapi.yml
- filename: soda-co-discovered-datasets-api-openapi.yml
  format: yaml
  label: Soda Discovered Datasets API
  slug: soda-co-discovered-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-discovered-datasets-api-openapi.yml
- filename: soda-co-incidents-api-openapi.yml
  format: yaml
  label: Soda Incidents API
  slug: soda-co-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-incidents-api-openapi.yml
- filename: soda-co-notification-rules-api-openapi.yml
  format: yaml
  label: Soda Notification Rules API
  slug: soda-co-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-notification-rules-api-openapi.yml
- filename: soda-co-runners-api-openapi.yml
  format: yaml
  label: Soda Runners API
  slug: soda-co-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-runners-api-openapi.yml
- filename: soda-co-scans-api-openapi.yml
  format: yaml
  label: Soda Scans API
  slug: soda-co-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-scans-api-openapi.yml
- filename: soda-co-secrets-api-openapi.yml
  format: yaml
  label: Soda Secrets API
  slug: soda-co-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-secrets-api-openapi.yml
- filename: soda-co-users-api-openapi.yml
  format: yaml
  label: Soda Users API
  slug: soda-co-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-users-api-openapi.yml
- filename: soda-co-utility-api-openapi.yml
  format: yaml
  label: Soda Utility API
  slug: soda-co-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/openapi/soda-co-utility-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Soda Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Soda
provider_slug: soda-co
scheme_count: 1
schemes:
- description: 'Base64-encoded API key ID and secret: base64(api_key_id:api_key_secret)'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/soda-cloud-rest-api.json
  type: http
slug: soda-co-authentication
source_filename: soda-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soda-cloud-rest-api.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Base64-encoded API key ID and secret: base64(api_key_id:api_key_secret)'\n  sources:\n  - openapi/soda-cloud-rest-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-co/refs/heads/main/authentication/soda-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Quality
- Data Observability
- Data Contracts
- Data Testing
- Data Monitoring
- Data Engineering
---
