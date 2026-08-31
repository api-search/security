---
api_key_in:
- header
api_specs:
- filename: acceldata-alerts-api-openapi.yml
  format: yaml
  label: Acceldata Alerts API
  slug: acceldata-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-alerts-api-openapi.yml
- filename: acceldata-data-quality-rules-api-openapi.yml
  format: yaml
  label: Acceldata Data Quality Rules API
  slug: acceldata-data-quality-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-data-quality-rules-api-openapi.yml
- filename: acceldata-datasets-api-openapi.yml
  format: yaml
  label: Acceldata Datasets API
  slug: acceldata-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-datasets-api-openapi.yml
- filename: acceldata-lineage-api-openapi.yml
  format: yaml
  label: Acceldata Lineage API
  slug: acceldata-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-lineage-api-openapi.yml
- filename: acceldata-pipeline-jobs-api-openapi.yml
  format: yaml
  label: Acceldata Pipeline Jobs API
  slug: acceldata-pipeline-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-pipeline-jobs-api-openapi.yml
- filename: acceldata-roles-api-openapi.yml
  format: yaml
  label: Acceldata Roles API
  slug: acceldata-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-roles-api-openapi.yml
- filename: acceldata-users-api-openapi.yml
  format: yaml
  label: Acceldata Users API
  slug: acceldata-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/acceldata-users-api-openapi.yml
- filename: acceldata-catalog-api-openapi.json
  format: json
  label: Acceldata Catalog API
  slug: acceldata-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-catalog-api-openapi.json
- filename: acceldata-administration-api-openapi.json
  format: json
  label: Acceldata Administration API
  slug: acceldata-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-administration-api-openapi.json
- filename: acceldata-tags-api-openapi.json
  format: json
  label: Acceldata Tag Services API
  slug: acceldata-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/openapi/_original/acceldata-tags-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Acceldata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acceldata secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Acceldata
provider_slug: acceldata
scheme_count: 2
schemes:
- description: Public API access key generated from the ADOC UI under Control Center > Security > API Keys. Sent as a bare header value on every request.
  in: header
  name: accessKey
  parameter: accessKey
  required: true
  sources:
  - https://docs.acceldata.io/api/authentication
  - openapi/_original/acceldata-catalog-api-openapi.json
  - openapi/_original/acceldata-tags-api-openapi.json
  type: apiKey
- description: Private API secret paired with accessKey. Issued once at key-generation time and not retrievable afterwards. Keys carry an operator-set expiry date.
  in: header
  name: secretKey
  parameter: secretKey
  required: true
  sources:
  - https://docs.acceldata.io/api/authentication
  - openapi/_original/acceldata-catalog-api-openapi.json
  - openapi/_original/acceldata-tags-api-openapi.json
  type: apiKey
slug: acceldata-authentication
source_filename: acceldata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.acceldata.io/api/authentication\ndocs: https://docs.acceldata.io/api/authentication\nkeys_docs: https://docs.acceldata.io/documentation/api-keys\nnote: >-\n  Upgraded from a derived profile that read X-API-Key out of an API-Evangelist-authored\n  spec. Acceldata's published API reference and its first-party OpenAPI documents\n  (documentation.acceldata.io/docs/acceldata/specs/*) both carry a two-header key PAIR —\n  accessKey and secretKey — declared as required header PARAMETERS on every operation\n  rather than as an OpenAPI securityScheme. No securitySchemes block is present in any\n  of the three published specs, and no top-level security requirement is declared.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  key_pair: true\n  oauth2: false\n  scheme_declared_in_spec: false\nschemes:\n- name: accessKey\n  type: apiKey\n  in: header\n  parameter: accessKey\n  required: true\n  description: >-\n\
  \    Public API access key generated from the ADOC UI under Control Center > Security >\n    API Keys. Sent as a bare header value on every request.\n  sources:\n  - https://docs.acceldata.io/api/authentication\n  - openapi/_original/acceldata-catalog-api-openapi.json\n  - openapi/_original/acceldata-tags-api-openapi.json\n- name: secretKey\n  type: apiKey\n  in: header\n  parameter: secretKey\n  required: true\n  description: >-\n    Private API secret paired with accessKey. Issued once at key-generation time and not\n    retrievable afterwards. Keys carry an operator-set expiry date.\n  sources:\n  - https://docs.acceldata.io/api/authentication\n  - openapi/_original/acceldata-catalog-api-openapi.json\n  - openapi/_original/acceldata-tags-api-openapi.json\nkey_management:\n  issued_from: ADOC UI — Control Center > Security > API Keys\n  rotation: >-\n    Keys are created with an explicit Validity Date and become invalid after it. The\n    Administration API exposes programmatic issue/revoke\
  \ operations.\n  programmatic_operations:\n  - createApiKey\n  - revokeApiKey\n  - listApiKeys\n  secret_shown_once: true\n  docs: https://docs.acceldata.io/documentation/api-keys\nrequired_headers:\n- name: accessKey\n  type: string\n- name: secretKey\n  type: string\n- name: accept\n  type: string\n  value: application/json\n- name: content-type\n  type: string\n  value: application/json\n  applies_to: requests with a body\noauth:\n- surface: documentation MCP server\n  issuer: https://documentation.acceldata.io\n  metadata: https://documentation.acceldata.io/.well-known/oauth-authorization-server\n  grant_types:\n  - authorization_code\n  code_challenge_methods:\n  - S256\n  scopes:\n  - mcp\n  note: >-\n    This OAuth authorization server protects the documentation MCP endpoint\n    (https://documentation.acceldata.io/mcp/rpc), not the ADOC platform APIs. The MCP\n    endpoint also answers anonymously today (tools/list returned 200 with no token).\ntenancy:\n  model: per-customer ADOC\
  \ deployment\n  note: >-\n    The published specs declare no servers[] block. Acceldata's own docs give the base as\n    https://<HOST>/catalog-server/api/... and the Python SDK takes url=\"https://<your-adoc-url>\",\n    so the host is the customer's own ADOC control-plane hostname, supplied by an administrator.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/authentication/acceldata-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
---
