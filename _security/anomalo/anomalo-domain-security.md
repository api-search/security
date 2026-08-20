---
api_specs:
- filename: anomalo-public-api-openapi.yml
  format: yaml
  label: Anomalo Public API
  slug: anomalo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomalo/refs/heads/main/openapi/anomalo-public-api-openapi.yml
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
- Data Quality
- Data Observability
- Data Monitoring
- Anomaly Detection
- Data Governance
- Data Lineage
- Data Profiling
- Data Validation
- Data Engineering
- Machine-Learning
- Snowflake
- Databricks
- BigQuery
- Enterprise Data
- MCP
- agent-native
---
