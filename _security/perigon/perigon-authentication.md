---
anonymous_access: false
api_key_in: []
api_specs:
- filename: perigon-ai-advanced-search-api-openapi.yml
  format: yaml
  label: Perigon AI & Advanced Search API
  slug: perigon-ai-advanced-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-ai-advanced-search-api-openapi.yml
- filename: perigon-contact-points-api-openapi.yml
  format: yaml
  label: Perigon Contact Points API
  slug: perigon-contact-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-contact-points-api-openapi.yml
- filename: perigon-monitors-api-openapi.yml
  format: yaml
  label: Perigon Monitors API
  slug: perigon-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-monitors-api-openapi.yml
- filename: perigon-news-stories-api-openapi.yml
  format: yaml
  label: Perigon News & Stories API
  slug: perigon-news-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-news-stories-api-openapi.yml
- filename: perigon-source-groups-api-openapi.yml
  format: yaml
  label: Perigon Source Groups API
  slug: perigon-source-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-source-groups-api-openapi.yml
- filename: perigon-supplemental-endpoints-api-openapi.yml
  format: yaml
  label: Perigon Supplemental Endpoints API
  slug: perigon-supplemental-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-supplemental-endpoints-api-openapi.yml
- filename: perigon-utilities-api-openapi.yml
  format: yaml
  label: Perigon Utilities API
  slug: perigon-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-utilities-api-openapi.yml
- filename: perigon-watchlists-api-openapi.yml
  format: yaml
  label: Perigon Watchlists API
  slug: perigon-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-watchlists-api-openapi.yml
- filename: perigon-wikipedia-api-openapi.yml
  format: yaml
  label: Perigon Wikipedia API
  slug: perigon-wikipedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-wikipedia-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Perigon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perigon declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Perigon
provider_slug: perigon
scheme_count: 3
schemes:
- header: Authorization
  in: header
  name: apiKeyAuth
  preferred: true
  scheme: bearer
  source: openapi securitySchemes
  type: http
- header: x-api-key
  in: header
  name: x-api-key
  source: https://perigon.io/docs/api/account-usage
  type: apiKey
- in: query
  name: apiKey
  parameter: apiKey
  source: https://perigon.io/docs/api/account-usage
  type: apiKey
slug: perigon-authentication
source_filename: perigon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: https://perigon.io/docs/api/authentication\ndocs: https://perigon.io/docs/api/authentication\nsummary: 'API key only. Perigon checks for the key in order: ?apiKey= query parameter, x-api-key header, Authorization:\n  Bearer header. Keys are created at https://perigon.io/dev/keys after browser sign-up; agent-readable instructions\n  at https://perigon.io/auth.md. OAuth metadata documents (RFC 9728 / RFC 8414) describe dashboard login (Google\n  OAuth, password grant) and an agent_auth block, not delegated API scopes.'\nschemes:\n- name: apiKeyAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  source: openapi securitySchemes\n  preferred: true\n- name: x-api-key\n  type: apiKey\n  in: header\n  header: x-api-key\n  source: https://perigon.io/docs/api/account-usage\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  source: https://perigon.io/docs/api/account-usage\nkey_management:\n\
  \  create: https://perigon.io/dev/keys\n  register: https://perigon.io/sign-up\n  revocation: disable or delete keys at https://perigon.io/dev/keys\n  validate: GET /v1/limits?apiKeys= checks up to 50 keys\ndiscovery:\n- https://perigon.io/.well-known/oauth-protected-resource\n- https://perigon.io/.well-known/oauth-authorization-server\n- https://perigon.io/auth.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/authentication/perigon-authentication.yml
summary_line: 3 schemes
tags:
- Company
- News
- Media Monitoring
- Search
- Artificial Intelligence
- Data
- MCP
- Webhook
---
