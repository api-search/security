---
api_key_in:
- header
api_specs:
- filename: apache-guacamole-active-connections-api-openapi.yml
  format: yaml
  label: Apache Guacamole Active Connections API
  slug: apache-guacamole-active-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-active-connections-api-openapi.yml
- filename: apache-guacamole-authentication-api-openapi.yml
  format: yaml
  label: Apache Guacamole Authentication API
  slug: apache-guacamole-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-authentication-api-openapi.yml
- filename: apache-guacamole-connections-api-openapi.yml
  format: yaml
  label: Apache Guacamole Connections API
  slug: apache-guacamole-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-connections-api-openapi.yml
- filename: apache-guacamole-history-api-openapi.yml
  format: yaml
  label: Apache Guacamole History API
  slug: apache-guacamole-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-history-api-openapi.yml
- filename: apache-guacamole-user-groups-api-openapi.yml
  format: yaml
  label: Apache Guacamole User Groups API
  slug: apache-guacamole-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-user-groups-api-openapi.yml
- filename: apache-guacamole-users-api-openapi.yml
  format: yaml
  label: Apache Guacamole Users API
  slug: apache-guacamole-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apache Guacamole Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Guacamole secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Guacamole
provider_slug: apache-guacamole
scheme_count: 1
schemes:
- description: Authentication token obtained from POST /api/tokens
  in: header
  name: GuacamoleToken
  parameter: Guacamole-Token
  sources:
  - openapi/apache-guacamole-rest-openapi.yml
  type: apiKey
slug: apache-guacamole-authentication
source_filename: apache-guacamole-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-guacamole-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: GuacamoleToken\n  type: apiKey\n  in: header\n  parameter: Guacamole-Token\n  description: Authentication token obtained from POST /api/tokens\n  sources:\n  - openapi/apache-guacamole-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/authentication/apache-guacamole-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
---
