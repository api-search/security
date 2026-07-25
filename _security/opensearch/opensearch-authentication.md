---
api_key_in: []
api_specs:
- filename: opensearch-account-api-openapi.yml
  format: yaml
  label: OpenSearch Account API
  slug: opensearch-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-account-api-openapi.yml
- filename: opensearch-action-groups-api-openapi.yml
  format: yaml
  label: OpenSearch Action Groups API
  slug: opensearch-action-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-action-groups-api-openapi.yml
- filename: opensearch-allowlist-api-openapi.yml
  format: yaml
  label: OpenSearch Allowlist API
  slug: opensearch-allowlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-allowlist-api-openapi.yml
- filename: opensearch-audit-api-openapi.yml
  format: yaml
  label: OpenSearch Audit API
  slug: opensearch-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-audit-api-openapi.yml
- filename: opensearch-cache-api-openapi.yml
  format: yaml
  label: OpenSearch Cache API
  slug: opensearch-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-cache-api-openapi.yml
- filename: opensearch-certificates-api-openapi.yml
  format: yaml
  label: OpenSearch Certificates API
  slug: opensearch-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-certificates-api-openapi.yml
- filename: opensearch-health-api-openapi.yml
  format: yaml
  label: OpenSearch Health API
  slug: opensearch-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-health-api-openapi.yml
- filename: opensearch-internal-users-api-openapi.yml
  format: yaml
  label: OpenSearch Internal Users API
  slug: opensearch-internal-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-internal-users-api-openapi.yml
- filename: opensearch-nodes-dn-api-openapi.yml
  format: yaml
  label: OpenSearch Nodes DN API
  slug: opensearch-nodes-dn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-nodes-dn-api-openapi.yml
- filename: opensearch-role-mappings-api-openapi.yml
  format: yaml
  label: OpenSearch Role Mappings API
  slug: opensearch-role-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-role-mappings-api-openapi.yml
- filename: opensearch-roles-api-openapi.yml
  format: yaml
  label: OpenSearch Roles API
  slug: opensearch-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-roles-api-openapi.yml
- filename: opensearch-security-config-api-openapi.yml
  format: yaml
  label: OpenSearch Security Config API
  slug: opensearch-security-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-security-config-api-openapi.yml
- filename: opensearch-ssl-info-api-openapi.yml
  format: yaml
  label: OpenSearch SSL Info API
  slug: opensearch-ssl-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-ssl-info-api-openapi.yml
- filename: opensearch-tenants-api-openapi.yml
  format: yaml
  label: OpenSearch Tenants API
  slug: opensearch-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-tenants-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opensearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenSearch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenSearch
provider_slug: opensearch
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/opensearch-security-openapi.yml
  type: http
slug: opensearch-authentication
source_filename: opensearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opensearch-security-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/opensearch-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/authentication/opensearch-authentication.yml
summary_line: http · 1 scheme
tags:
- Search
- Analytics
- Observability
- Open Source
- Security
---
