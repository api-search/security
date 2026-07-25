---
api_key_in: []
api_specs:
- filename: oracle-enterprise-manager-blackouts-api-openapi.yml
  format: yaml
  label: Oracle Enterprise Manager Blackouts API
  slug: oracle-enterprise-manager-blackouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/openapi/oracle-enterprise-manager-blackouts-api-openapi.yml
- filename: oracle-enterprise-manager-events-api-openapi.yml
  format: yaml
  label: Oracle Enterprise Manager Events API
  slug: oracle-enterprise-manager-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/openapi/oracle-enterprise-manager-events-api-openapi.yml
- filename: oracle-enterprise-manager-global-target-properties-api-openapi.yml
  format: yaml
  label: Oracle Enterprise Manager Global Target Properties API
  slug: oracle-enterprise-manager-global-target-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/openapi/oracle-enterprise-manager-global-target-properties-api-openapi.yml
- filename: oracle-enterprise-manager-incidents-api-openapi.yml
  format: yaml
  label: Oracle Enterprise Manager Incidents API
  slug: oracle-enterprise-manager-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/openapi/oracle-enterprise-manager-incidents-api-openapi.yml
- filename: oracle-enterprise-manager-metrics-api-openapi.yml
  format: yaml
  label: Oracle Enterprise Manager Metrics API
  slug: oracle-enterprise-manager-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/openapi/oracle-enterprise-manager-metrics-api-openapi.yml
- filename: oracle-enterprise-manager-targets-api-openapi.yml
  format: yaml
  label: Oracle Enterprise Manager Targets API
  slug: oracle-enterprise-manager-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/openapi/oracle-enterprise-manager-targets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Enterprise Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Enterprise Manager secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using Enterprise Manager administrator credentials. All API requests must include valid credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-enterprise-manager-cloud-control-openapi.yml
  type: http
slug: oracle-enterprise-manager-authentication
source_filename: oracle-enterprise-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-enterprise-manager-cloud-control-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Enterprise Manager administrator credentials.\n    All API requests must include valid credentials.\n  sources:\n  - openapi/oracle-enterprise-manager-cloud-control-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/authentication/oracle-enterprise-manager-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
---
