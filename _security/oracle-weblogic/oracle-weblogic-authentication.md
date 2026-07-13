---
api_key_in: []
api_specs:
- filename: oracle-weblogic-management-openapi.yml
  format: yaml
  label: WebLogic RESTful Management Services API
  slug: weblogic-restful-management-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/openapi/oracle-weblogic-management-openapi.yml
- filename: oracle-weblogic-monitoring-openapi.yml
  format: yaml
  label: WebLogic Monitoring and Diagnostics API
  slug: weblogic-monitoring-and-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/openapi/oracle-weblogic-monitoring-openapi.yml
- filename: oracle-weblogic-deployment-openapi.yml
  format: yaml
  label: WebLogic Deployment API
  slug: weblogic-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/openapi/oracle-weblogic-deployment-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Weblogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle WebLogic Server secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oracle WebLogic Server
provider_slug: oracle-weblogic
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Deployer role required for deployment operations, Operator role for lifecycle operations.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-weblogic-deployment-openapi.yml
  - openapi/oracle-weblogic-management-openapi.yml
  - openapi/oracle-weblogic-monitoring-openapi.yml
  type: http
slug: oracle-weblogic-authentication
source_filename: oracle-weblogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-weblogic-deployment-openapi.yml, openapi/oracle-weblogic-management-openapi.yml,\n  openapi/oracle-weblogic-monitoring-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Deployer role required for deployment operations,\n    Operator role for lifecycle operations.\n  sources:\n  - openapi/oracle-weblogic-deployment-openapi.yml\n  - openapi/oracle-weblogic-management-openapi.yml\n  - openapi/oracle-weblogic-monitoring-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/authentication/oracle-weblogic-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
---
