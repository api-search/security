---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: clickhouse-clickhouse-http-interface-api-openapi.yml
  format: yaml
  label: ClickHouse ClickHouse HTTP Interface API
  slug: clickhouse-clickhouse-http-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-clickhouse-http-interface-api-openapi.yml
- filename: clickhouse-ping-api-openapi.yml
  format: yaml
  label: ClickHouse Ping API
  slug: clickhouse-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-ping-api-openapi.yml
- filename: clickhouse-play-api-openapi.yml
  format: yaml
  label: ClickHouse Play API
  slug: clickhouse-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-play-api-openapi.yml
- filename: clickhouse-replicas-status-api-openapi.yml
  format: yaml
  label: ClickHouse Replicas Status API
  slug: clickhouse-replicas-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-replicas-status-api-openapi.yml
- filename: clickhouse-cloud-api-openapi.json
  format: json
  label: ClickHouse Cloud API
  slug: clickhouse-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-cloud-api-openapi.json
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Clickhouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClickHouse secures its APIs with http, apiKey, and oauth2 across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClickHouse
provider_slug: clickhouse
scheme_count: 0
schemes: []
slug: clickhouse-authentication
source_filename: clickhouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://clickhouse.com/docs/cloud/manage/openapi and https://clickhouse.com/docs/cloud/manage/api/api-overview,\n  reconciled against openapi/clickhouse-cloud-api-openapi.json (live spec fetched from\n  https://api.clickhouse.cloud/v1 on 2026-09-05), openapi/_original/clickhouse-openapi.yml (HTTP interface),\n  and the MCP discovery documents in well-known/\ndocs: https://clickhouse.com/docs/cloud/manage/openapi\nsummary:\n  types:\n    - http\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n    - query\nsurfaces:\n  - name: ClickHouse Cloud API\n    base: https://api.clickhouse.cloud/v1\n    schemes:\n      - name: basicAuth\n        type: http\n        scheme: basic\n        username: API key ID\n        password: API key secret\n        applies_to: all 148 operations\n        sources:\n          - openapi/clickhouse-cloud-api-openapi.json\n        example: 'curl --user $KEY_ID:$KEY_SECRET https://api.clickhouse.cloud/v1/organizations'\n\
  \    key_management:\n      issue: ClickHouse Cloud console -> API Keys -> New API Key\n      roles:\n        - name: developer\n          grants: read-only permissions for assigned services\n        - name: admin\n          grants: full read and write permissions\n      expiration: configurable per key\n      ip_allowlist: optional per key — a single IP or a CIDR range such as 203.0.113.0/24\n      keys_per_organization: 100\n      secret_display: >-\n        Key ID and key secret are shown once at creation and never again; ClickHouse tells you to store them\n        in a vault.\n      revocation: >-\n        Keys can be disabled or deleted from the API Keys page. Deletion is permanent and immediately cuts\n        off any service using the key.\n  - name: ClickHouse HTTP interface\n    base: 'http(s)://<host>:8123 (HTTPS 8443)'\n    schemes:\n      - name: basicAuth\n        type: http\n        scheme: basic\n        sources:\n          - openapi/_original/clickhouse-openapi.yml\n  \
  \    - name: clickhouseHeaders\n        type: apiKey\n        in: header\n        parameter: X-ClickHouse-User\n        companion: X-ClickHouse-Key\n        sources:\n          - openapi/_original/clickhouse-openapi.yml\n      - name: urlParameters\n        type: apiKey\n        in: query\n        parameter: user\n        companion: password\n        note: Credentials may also be passed as URL parameters — documented, but the weakest of the three.\n    docs: https://clickhouse.com/docs/en/interfaces/http\n  - name: ClickHouse Cloud remote MCP server\n    base: https://mcp.clickhouse.cloud/mcp\n    schemes:\n      - name: oauth2\n        type: oauth2\n        flow: authorization_code with PKCE (S256)\n        issuer: https://mcp.clickhouse.cloud\n        dynamic_registration: https://mcp.clickhouse.cloud/register\n        scopes:\n          - 'mcp:access'\n          - 'clickstack:access'\n          - openid\n          - profile\n          - email\n        sources:\n          - well-known/clickhouse-mcp-oauth-authorization-server.json\n\
  \          - well-known/clickhouse-mcp-oauth-protected-resource.json\n    detail: scopes/clickhouse-scopes.yml\nsso:\n  google: all plans\n  microsoft: all plans\n  saml: Enterprise plan only\n  mfa: all plans\n  source: https://clickhouse.com/pricing.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/authentication/clickhouse-authentication.yml
summary_line: http/apiKey/oauth2 · 0 schemes
tags:
- Analytics
- Cloud Database
- Column-Oriented
- Database
- OLAP
- Open-Source
- Real-Time
- SQL
---
