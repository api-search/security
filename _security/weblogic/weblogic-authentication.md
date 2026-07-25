---
api_key_in: []
api_specs:
- filename: weblogic-application-deployments-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Application Deployments API
  slug: weblogic-application-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-application-deployments-api-openapi.yml
- filename: weblogic-applications-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Applications API
  slug: weblogic-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-applications-api-openapi.yml
- filename: weblogic-clusters-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Clusters API
  slug: weblogic-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-clusters-api-openapi.yml
- filename: weblogic-data-sources-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Data Sources API
  slug: weblogic-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-data-sources-api-openapi.yml
- filename: weblogic-deployment-operations-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Deployment Operations API
  slug: weblogic-deployment-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-deployment-operations-api-openapi.yml
- filename: weblogic-diagnostics-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Diagnostics API
  slug: weblogic-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-diagnostics-api-openapi.yml
- filename: weblogic-domain-configuration-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Domain Configuration API
  slug: weblogic-domain-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-domain-configuration-api-openapi.yml
- filename: weblogic-domain-runtime-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Domain Runtime API
  slug: weblogic-domain-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-domain-runtime-api-openapi.yml
- filename: weblogic-edit-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Edit API
  slug: weblogic-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-edit-api-openapi.yml
- filename: weblogic-health-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Health API
  slug: weblogic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-health-api-openapi.yml
- filename: weblogic-jms-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs JMS API
  slug: weblogic-jms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-jms-api-openapi.yml
- filename: weblogic-library-deployments-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Library Deployments API
  slug: weblogic-library-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-library-deployments-api-openapi.yml
- filename: weblogic-lifecycle-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Lifecycle API
  slug: weblogic-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-lifecycle-api-openapi.yml
- filename: weblogic-server-configuration-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Server Configuration API
  slug: weblogic-server-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-server-configuration-api-openapi.yml
- filename: weblogic-server-runtime-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Server Runtime API
  slug: weblogic-server-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-server-runtime-api-openapi.yml
- filename: weblogic-servers-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Servers API
  slug: weblogic-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-servers-api-openapi.yml
- filename: weblogic-upload-api-openapi.yml
  format: yaml
  label: Oracle WebLogic Server APIs Upload API
  slug: weblogic-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-upload-api-openapi.yml
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
