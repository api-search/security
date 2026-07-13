---
api_key_in: []
api_specs:
- filename: weblogic-restful-management-services-openapi.yml
  format: yaml
  label: WebLogic RESTful Management Services API
  slug: weblogic-restful-management-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-restful-management-services-openapi.yml
- filename: weblogic-monitoring-diagnostics-openapi.yml
  format: yaml
  label: WebLogic Monitoring and Diagnostics API
  slug: weblogic-monitoring-and-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-monitoring-diagnostics-openapi.yml
- filename: weblogic-deployment-openapi.yml
  format: yaml
  label: WebLogic Deployment API
  slug: weblogic-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-deployment-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Weblogic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle WebLogic Server APIs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oracle WebLogic Server APIs
provider_slug: weblogic
scheme_count: 1
schemes:
- description: WebLogic Server administrator credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/weblogic-deployment-openapi.yml
  - openapi/weblogic-monitoring-diagnostics-openapi.yml
  - openapi/weblogic-restful-management-services-openapi.yml
  type: http
slug: weblogic-authentication
source_filename: weblogic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weblogic-deployment-openapi.yml, openapi/weblogic-monitoring-diagnostics-openapi.yml,\n  openapi/weblogic-restful-management-services-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: WebLogic Server administrator credentials\n  sources:\n  - openapi/weblogic-deployment-openapi.yml\n  - openapi/weblogic-monitoring-diagnostics-openapi.yml\n  - openapi/weblogic-restful-management-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/authentication/weblogic-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
- WebLogic
---
