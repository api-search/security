---
api_key_in:
- header
api_specs:
- filename: zuplo-api-keys-buckets-api-openapi.yml
  format: yaml
  label: Zuplo API Keys - Buckets API
  slug: zuplo-api-keys-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-api-keys-buckets-api-openapi.yml
- filename: zuplo-api-keys-consumers-api-openapi.yml
  format: yaml
  label: Zuplo API Keys - Consumers API
  slug: zuplo-api-keys-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-api-keys-consumers-api-openapi.yml
- filename: zuplo-api-keys-keys-api-openapi.yml
  format: yaml
  label: Zuplo API Keys - Keys API
  slug: zuplo-api-keys-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-api-keys-keys-api-openapi.yml
- filename: zuplo-api-keys-managers-api-openapi.yml
  format: yaml
  label: Zuplo API Keys - Managers API
  slug: zuplo-api-keys-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-api-keys-managers-api-openapi.yml
- filename: zuplo-audit-logs-api-openapi.yml
  format: yaml
  label: Zuplo Audit Logs API
  slug: zuplo-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-audit-logs-api-openapi.yml
- filename: zuplo-custom-domains-api-openapi.yml
  format: yaml
  label: Zuplo Custom Domains API
  slug: zuplo-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-custom-domains-api-openapi.yml
- filename: zuplo-deployments-api-openapi.yml
  format: yaml
  label: Zuplo Deployments API
  slug: zuplo-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-deployments-api-openapi.yml
- filename: zuplo-mcp-servers-api-openapi.yml
  format: yaml
  label: Zuplo MCP Servers API
  slug: zuplo-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-mcp-servers-api-openapi.yml
- filename: zuplo-openapi-api-openapi.yml
  format: yaml
  label: Zuplo Openapi API
  slug: zuplo-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-openapi-api-openapi.yml
- filename: zuplo-tunnel-services-api-openapi.yml
  format: yaml
  label: Zuplo Tunnel Services API
  slug: zuplo-tunnel-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-tunnel-services-api-openapi.yml
- filename: zuplo-tunnels-api-openapi.yml
  format: yaml
  label: Zuplo Tunnels API
  slug: zuplo-tunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-tunnels-api-openapi.yml
- filename: zuplo-variables-api-openapi.yml
  format: yaml
  label: Zuplo Variables API
  slug: zuplo-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-variables-api-openapi.yml
- filename: zuplo-who-am-i-api-openapi.yml
  format: yaml
  label: Zuplo Who Am I API
  slug: zuplo-who-am-i-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-who-am-i-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zuplo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zuplo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zuplo
provider_slug: zuplo
scheme_count: 1
schemes:
- description: 'API key authentication. Format: Bearer {api-key}'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/zuplo-openapi.yml
  type: apiKey
slug: zuplo-authentication
source_filename: zuplo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zuplo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication. Format: Bearer {api-key}'\n  sources:\n  - openapi/zuplo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/authentication/zuplo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Gateway
- API Management
- Gateways
- Platform
---
