---
api_key_in:
- header
api_specs:
- filename: apollo-config-apps-api-openapi.yml
  format: yaml
  label: Apollo Config Apps API
  slug: apollo-config-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/openapi/apollo-config-apps-api-openapi.yml
- filename: apollo-config-clusters-api-openapi.yml
  format: yaml
  label: Apollo Config Clusters API
  slug: apollo-config-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/openapi/apollo-config-clusters-api-openapi.yml
- filename: apollo-config-items-api-openapi.yml
  format: yaml
  label: Apollo Config Items API
  slug: apollo-config-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/openapi/apollo-config-items-api-openapi.yml
- filename: apollo-config-namespaces-api-openapi.yml
  format: yaml
  label: Apollo Config Namespaces API
  slug: apollo-config-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/openapi/apollo-config-namespaces-api-openapi.yml
- filename: apollo-config-releases-api-openapi.yml
  format: yaml
  label: Apollo Config Releases API
  slug: apollo-config-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/openapi/apollo-config-releases-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apollo Config Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apollo Config secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apollo Config
provider_slug: apollo-config
scheme_count: 1
schemes:
- description: Apollo Portal open API token
  in: header
  name: PortalToken
  parameter: Authorization
  sources:
  - openapi/apollo-open-api.yml
  type: apiKey
slug: apollo-config-authentication
source_filename: apollo-config-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apollo-open-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PortalToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Apollo Portal open API token\n  sources:\n  - openapi/apollo-open-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/authentication/apollo-config-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Apache 2.0
- Configuration Management
- Ctrip
- Distributed Systems
- Java
- Microservices
- Open-Source
- Real-Time Configuration
---
