---
api_specs:
- filename: anomalo-access-groups-api-openapi.yml
  format: yaml
  label: Anomalo Access Groups API
  slug: anomalo-access-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-access-groups-api-openapi.yml
- filename: anomalo-api-keys-api-openapi.yml
  format: yaml
  label: Anomalo API Keys API
  slug: anomalo-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-api-keys-api-openapi.yml
- filename: anomalo-check-runs-api-openapi.yml
  format: yaml
  label: Anomalo Check Runs API
  slug: anomalo-check-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-check-runs-api-openapi.yml
- filename: anomalo-checks-api-openapi.yml
  format: yaml
  label: Anomalo Checks API
  slug: anomalo-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-checks-api-openapi.yml
- filename: anomalo-document-collections-api-openapi.yml
  format: yaml
  label: Anomalo Document Collections API
  slug: anomalo-document-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-document-collections-api-openapi.yml
- filename: anomalo-documents-api-openapi.yml
  format: yaml
  label: Anomalo Documents API
  slug: anomalo-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-documents-api-openapi.yml
- filename: anomalo-exports-api-openapi.yml
  format: yaml
  label: Anomalo Exports API
  slug: anomalo-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-exports-api-openapi.yml
- filename: anomalo-issues-api-openapi.yml
  format: yaml
  label: Anomalo Issues API
  slug: anomalo-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-issues-api-openapi.yml
- filename: anomalo-labels-api-openapi.yml
  format: yaml
  label: Anomalo Labels API
  slug: anomalo-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-labels-api-openapi.yml
- filename: anomalo-lineage-api-openapi.yml
  format: yaml
  label: Anomalo Lineage API
  slug: anomalo-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-lineage-api-openapi.yml
- filename: anomalo-notification-channels-api-openapi.yml
  format: yaml
  label: Anomalo Notification Channels API
  slug: anomalo-notification-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-notification-channels-api-openapi.yml
- filename: anomalo-organizations-api-openapi.yml
  format: yaml
  label: Anomalo Organizations API
  slug: anomalo-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-organizations-api-openapi.yml
- filename: anomalo-sensitive-columns-api-openapi.yml
  format: yaml
  label: Anomalo Sensitive Columns API
  slug: anomalo-sensitive-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-sensitive-columns-api-openapi.yml
- filename: anomalo-system-api-openapi.yml
  format: yaml
  label: Anomalo System API
  slug: anomalo-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-system-api-openapi.yml
- filename: anomalo-tables-api-openapi.yml
  format: yaml
  label: Anomalo Tables API
  slug: anomalo-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-tables-api-openapi.yml
- filename: anomalo-tasks-api-openapi.yml
  format: yaml
  label: Anomalo Tasks API
  slug: anomalo-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-tasks-api-openapi.yml
- filename: anomalo-users-api-openapi.yml
  format: yaml
  label: Anomalo Users API
  slug: anomalo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-users-api-openapi.yml
- filename: anomalo-warehouses-api-openapi.yml
  format: yaml
  label: Anomalo Warehouses API
  slug: anomalo-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-warehouses-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anomalo.com
  spf: false
hosts:
- cert_expires: Oct  6 04:38:55 2026 GMT
  host: www.anomalo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 08:29:27 2026 GMT
  host: app.anomalo.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anomalo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anomalo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Anomalo
provider_slug: anomalo
slug: anomalo-domain-security
source_filename: anomalo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anomalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:38:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.anomalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 08:29:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: anomalo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/security/anomalo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- data-quality
- data-observability
- data-monitoring
- anomaly-detection
- data-governance
- data-lineage
- data-profiling
- data-validation
- data-engineering
- machine-learning
- snowflake
- databricks
- bigquery
- enterprise-data
- MCP
- agent-native
---
