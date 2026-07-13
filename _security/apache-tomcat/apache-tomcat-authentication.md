---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Tomcat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Tomcat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Tomcat
provider_slug: apache-tomcat
scheme_count: 1
schemes:
- description: HTTP Basic authentication; user must hold the `manager-script` role
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-tomcat-openapi.yml
  type: http
slug: apache-tomcat-authentication
source_filename: apache-tomcat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-tomcat-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication; user must hold the `manager-script` role\n  sources:\n  - openapi/apache-tomcat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-tomcat/refs/heads/main/authentication/apache-tomcat-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Server
- Java
- JSP
- Open Source
- Servlet
- Web Server
---
