---
api_key_in:
- header
api_specs:
- filename: apache-apisix-consumer-groups-api-openapi.yml
  format: yaml
  label: Apache APISIX Consumer Groups API
  slug: apache-apisix-consumer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-consumer-groups-api-openapi.yml
- filename: apache-apisix-consumers-api-openapi.yml
  format: yaml
  label: Apache APISIX Consumers API
  slug: apache-apisix-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-consumers-api-openapi.yml
- filename: apache-apisix-diagnostics-api-openapi.yml
  format: yaml
  label: Apache APISIX Diagnostics API
  slug: apache-apisix-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-diagnostics-api-openapi.yml
- filename: apache-apisix-global-rules-api-openapi.yml
  format: yaml
  label: Apache APISIX Global Rules API
  slug: apache-apisix-global-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-global-rules-api-openapi.yml
- filename: apache-apisix-health-check-api-openapi.yml
  format: yaml
  label: Apache APISIX Health Check API
  slug: apache-apisix-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-health-check-api-openapi.yml
- filename: apache-apisix-introspection-api-openapi.yml
  format: yaml
  label: Apache APISIX Introspection API
  slug: apache-apisix-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-introspection-api-openapi.yml
- filename: apache-apisix-plugin-configs-api-openapi.yml
  format: yaml
  label: Apache APISIX Plugin Configs API
  slug: apache-apisix-plugin-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-plugin-configs-api-openapi.yml
- filename: apache-apisix-plugin-metadata-api-openapi.yml
  format: yaml
  label: Apache APISIX Plugin Metadata API
  slug: apache-apisix-plugin-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-plugin-metadata-api-openapi.yml
- filename: apache-apisix-plugins-api-openapi.yml
  format: yaml
  label: Apache APISIX Plugins API
  slug: apache-apisix-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-plugins-api-openapi.yml
- filename: apache-apisix-protos-api-openapi.yml
  format: yaml
  label: Apache APISIX Protos API
  slug: apache-apisix-protos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-protos-api-openapi.yml
- filename: apache-apisix-routes-api-openapi.yml
  format: yaml
  label: Apache APISIX Routes API
  slug: apache-apisix-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-routes-api-openapi.yml
- filename: apache-apisix-schema-api-openapi.yml
  format: yaml
  label: Apache APISIX Schema API
  slug: apache-apisix-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-schema-api-openapi.yml
- filename: apache-apisix-secrets-api-openapi.yml
  format: yaml
  label: Apache APISIX Secrets API
  slug: apache-apisix-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-secrets-api-openapi.yml
- filename: apache-apisix-services-api-openapi.yml
  format: yaml
  label: Apache APISIX Services API
  slug: apache-apisix-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-services-api-openapi.yml
- filename: apache-apisix-ssl-api-openapi.yml
  format: yaml
  label: Apache APISIX SSL API
  slug: apache-apisix-ssl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-ssl-api-openapi.yml
- filename: apache-apisix-stream-routes-api-openapi.yml
  format: yaml
  label: Apache APISIX Stream Routes API
  slug: apache-apisix-stream-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-stream-routes-api-openapi.yml
- filename: apache-apisix-upstreams-api-openapi.yml
  format: yaml
  label: Apache APISIX Upstreams API
  slug: apache-apisix-upstreams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-upstreams-api-openapi.yml
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
- Cloud-Native
- Kubernetes
- Lua
- NGINX
- Open-Source
- Traffic Management
---
