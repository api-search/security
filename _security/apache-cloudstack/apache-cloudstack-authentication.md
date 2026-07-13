---
api_key_in:
- query
api_specs:
- filename: apache-cloudstack-api-openapi.yaml
  format: yaml
  label: Apache CloudStack API
  slug: apache-cloudstack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/openapi/apache-cloudstack-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apache Cloudstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache CloudStack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
scheme_count: 1
schemes:
- description: CloudStack API key for HMAC-SHA1 signed request authentication.
  in: query
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/apache-cloudstack-api-openapi.yaml
  type: apiKey
slug: apache-cloudstack-authentication
source_filename: apache-cloudstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-cloudstack-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: CloudStack API key for HMAC-SHA1 signed request authentication.\n  sources:\n  - openapi/apache-cloudstack-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/authentication/apache-cloudstack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
---
