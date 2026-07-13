---
api_key_in: []
api_specs:
- filename: oracle-enterprise-manager-cloud-control-openapi.yml
  format: yaml
  label: Oracle Enterprise Manager Cloud Control REST API
  slug: oracle-enterprise-manager-cloud-control-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/openapi/oracle-enterprise-manager-cloud-control-openapi.yml
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
