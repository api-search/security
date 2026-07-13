---
api_key_in: []
api_specs:
- filename: apache-atlas-rest-openapi.yaml
  format: yaml
  label: Apache Atlas REST API
  slug: apache-atlas-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/openapi/apache-atlas-rest-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Atlas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Atlas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Atlas
provider_slug: apache-atlas
scheme_count: 1
schemes:
- description: HTTP Basic authentication with Atlas admin credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-atlas-rest-openapi.yaml
  type: http
slug: apache-atlas-authentication
source_filename: apache-atlas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-atlas-rest-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with Atlas admin credentials.\n  sources:\n  - openapi/apache-atlas-rest-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/authentication/apache-atlas-authentication.yml
summary_line: http · 1 scheme
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
---
