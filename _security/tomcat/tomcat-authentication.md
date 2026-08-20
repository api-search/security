---
api_key_in: []
api_specs:
- filename: tomcat-applications-api-openapi.yml
  format: yaml
  label: Apache Tomcat Applications API
  slug: tomcat-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-applications-api-openapi.yml
- filename: tomcat-configuration-api-openapi.yml
  format: yaml
  label: Apache Tomcat Configuration API
  slug: tomcat-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-configuration-api-openapi.yml
- filename: tomcat-diagnostics-api-openapi.yml
  format: yaml
  label: Apache Tomcat Diagnostics API
  slug: tomcat-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-diagnostics-api-openapi.yml
- filename: tomcat-jmx-api-openapi.yml
  format: yaml
  label: Apache Tomcat JMX API
  slug: tomcat-jmx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-jmx-api-openapi.yml
- filename: tomcat-sessions-api-openapi.yml
  format: yaml
  label: Apache Tomcat Sessions API
  slug: tomcat-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-sessions-api-openapi.yml
- filename: tomcat-ssl-api-openapi.yml
  format: yaml
  label: Apache Tomcat SSL API
  slug: tomcat-ssl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-ssl-api-openapi.yml
- filename: tomcat-status-api-openapi.yml
  format: yaml
  label: Apache Tomcat Status API
  slug: tomcat-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tomcat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Tomcat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Tomcat
provider_slug: tomcat
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. User must have appropriate role in tomcat-users.xml: manager-script for text interface, manager-jmx for JMX proxy.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tomcat-manager-openapi.yml
  type: http
slug: tomcat-authentication
source_filename: tomcat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tomcat-manager-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic authentication. User must have appropriate role in tomcat-users.xml:\n    manager-script for text interface, manager-jmx for JMX proxy.'\n  sources:\n  - openapi/tomcat-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/authentication/tomcat-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Server
- Java
- Servlet Container
- Web Server
- Open-Source
- Apache
---
