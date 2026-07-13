---
api_key_in:
- header
api_specs:
- filename: apache-apisix-admin-api-openapi.yml
  format: yaml
  label: Apache APISIX Admin API
  slug: apache-apisix-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-admin-api-openapi.yml
- filename: apache-apisix-control-api-openapi.yml
  format: yaml
  label: Apache APISIX Control API
  slug: apache-apisix-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-control-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apache Apisix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache APISIX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache APISIX
provider_slug: apache-apisix
scheme_count: 1
schemes:
- description: Admin API key for authentication.
  in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/apache-apisix-admin-api-openapi.yml
  type: apiKey
slug: apache-apisix-authentication
source_filename: apache-apisix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-apisix-admin-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: Admin API key for authentication.\n  sources:\n  - openapi/apache-apisix-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/authentication/apache-apisix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
---
