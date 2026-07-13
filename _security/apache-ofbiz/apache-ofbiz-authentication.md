---
api_key_in: []
api_specs:
- filename: apache-ofbiz-rest-api-openapi.yaml
  format: yaml
  label: Apache OFBiz REST API
  slug: apache-ofbiz-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/openapi/apache-ofbiz-rest-api-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Ofbiz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache OFBiz secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
scheme_count: 2
schemes:
- description: HTTP Basic Auth used only for token acquisition at /auth/token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-ofbiz-rest-api-openapi.yaml
  type: http
- bearerFormat: JWT
  description: JWT Bearer token obtained from /auth/token. Required for all service endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apache-ofbiz-rest-api-openapi.yaml
  type: http
slug: apache-ofbiz-authentication
source_filename: apache-ofbiz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-ofbiz-rest-api-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth used only for token acquisition at /auth/token.\n  sources:\n  - openapi/apache-ofbiz-rest-api-openapi.yaml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT Bearer token obtained from /auth/token. Required for all service endpoints.\n  sources:\n  - openapi/apache-ofbiz-rest-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/authentication/apache-ofbiz-authentication.yml
summary_line: http · 2 schemes
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
---
