---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opensearch.org
  spf: true
hosts:
- cert_expires: Sep  7 13:20:42 2026 GMT
  host: opensearch.org
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: docs.opensearch.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opensearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSearch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenSearch
provider_slug: opensearch
slug: opensearch-domain-security
source_filename: opensearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opensearch.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:20:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: docs.opensearch.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opensearch.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/security/opensearch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Analytics
- Observability
- Open-Source
- Security
---
