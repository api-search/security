---
api_key_in: []
api_specs:
- filename: apache-struts-openapi.yml
  format: yaml
  label: Apache Struts REST Plugin
  slug: apache-struts-rest-plugin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-struts/refs/heads/main/openapi/apache-struts-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Struts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Struts secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Struts
provider_slug: apache-struts
scheme_count: 1
schemes:
- description: The REST plugin does not define authentication itself; authentication is typically applied via standard Struts interceptors (HTTP Basic, form login, container-managed, etc.).
  name: strutsInterceptor
  scheme: basic
  sources:
  - openapi/apache-struts-openapi.yml
  type: http
slug: apache-struts-authentication
source_filename: apache-struts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-struts-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: strutsInterceptor\n  type: http\n  scheme: basic\n  description: The REST plugin does not define authentication itself; authentication is typically\n    applied via standard Struts interceptors (HTTP Basic, form login, container-managed, etc.).\n  sources:\n  - openapi/apache-struts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-struts/refs/heads/main/authentication/apache-struts-authentication.yml
summary_line: http · 1 scheme
tags:
- Java
- MVC
- Web Applications
- Web Framework
- Open Source
---
