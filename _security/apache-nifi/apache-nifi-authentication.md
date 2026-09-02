---
api_key_in: []
api_specs:
- filename: apache-nifi-access-api-openapi.yml
  format: yaml
  label: Apache NiFi Access API
  slug: apache-nifi-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/openapi/apache-nifi-access-api-openapi.yml
- filename: apache-nifi-connections-api-openapi.yml
  format: yaml
  label: Apache NiFi Connections API
  slug: apache-nifi-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/openapi/apache-nifi-connections-api-openapi.yml
- filename: apache-nifi-controller-services-api-openapi.yml
  format: yaml
  label: Apache NiFi Controller Services API
  slug: apache-nifi-controller-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/openapi/apache-nifi-controller-services-api-openapi.yml
- filename: apache-nifi-flow-api-openapi.yml
  format: yaml
  label: Apache NiFi Flow API
  slug: apache-nifi-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/openapi/apache-nifi-flow-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Nifi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache NiFi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache NiFi
provider_slug: apache-nifi
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT issued by POST /access/token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apache-nifi-openapi.yml
  type: http
slug: apache-nifi-authentication
source_filename: apache-nifi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-nifi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT issued by POST /access/token\n  sources:\n  - openapi/apache-nifi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-nifi/refs/heads/main/authentication/apache-nifi-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Integration
- Dataflows
- ETL
- IoT
- Streaming
- Data Pipeline
---
