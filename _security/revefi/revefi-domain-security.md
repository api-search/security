---
api_specs:
- filename: revefi-create-a-custom-data-quality-monitor-api-openapi.yml
  format: yaml
  label: Revefi Create a Custom Data Quality Monitor API
  slug: revefi-create-a-custom-data-quality-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-create-a-custom-data-quality-monitor-api-openapi.yml
- filename: revefi-delete-an-existing-custom-data-quality-monitor-api-openapi.yml
  format: yaml
  label: Revefi Delete an existing Custom Data Quality Monitor API
  slug: revefi-delete-an-existing-custom-data-quality-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-delete-an-existing-custom-data-quality-monitor-api-openapi.yml
- filename: revefi-get-custom-data-quality-monitors-api-openapi.yml
  format: yaml
  label: Revefi Get Custom Data Quality Monitors API
  slug: revefi-get-custom-data-quality-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-get-custom-data-quality-monitors-api-openapi.yml
- filename: revefi-get-custom-data-quality-monitors-by-artifact-api-openapi.yml
  format: yaml
  label: Revefi Get Custom Data Quality Monitors by Artifact API
  slug: revefi-get-custom-data-quality-monitors-by-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-get-custom-data-quality-monitors-by-artifact-api-openapi.yml
- filename: revefi-run-monitors-api-openapi.yml
  format: yaml
  label: Revefi Run Monitors API
  slug: revefi-run-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-run-monitors-api-openapi.yml
- filename: revefi-update-an-existing-custom-data-quality-monitor-api-openapi.yml
  format: yaml
  label: Revefi Update an existing Custom Data Quality Monitor API
  slug: revefi-update-an-existing-custom-data-quality-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/openapi/revefi-update-an-existing-custom-data-quality-monitor-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revefi.com
  spf: true
hosts:
- cert_expires: Oct 14 20:33:50 2026 GMT
  host: revefi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: gateway.revefi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revefi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revefi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revefi
provider_slug: revefi
slug: revefi-domain-security
source_filename: revefi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.revefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: revefi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revefi/refs/heads/main/security/revefi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Data Quality
- Data Observability
- FinOps
- Cost Optimization
- Analytics
- Snowflake
- Databricks
- BigQuery
- Artificial Intelligence
- MCP
---
