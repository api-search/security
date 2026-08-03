---
api_specs:
- filename: bigeye-metadata-openapi.json
  format: json
  label: Bigeye Metadata API
  slug: bigeye-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-metadata-openapi.json
- filename: bigeye-observability-openapi.json
  format: json
  label: Bigeye Observability API
  slug: bigeye-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-observability-openapi.json
- filename: bigeye-sensitivity-openapi.json
  format: json
  label: Bigeye Sensitivity API
  slug: bigeye-sensitivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-sensitivity-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bigeye.com
  spf: true
hosts:
- cert_expires: Sep  9 08:44:19 2026 GMT
  host: www.bigeye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 04:51:23 2026 GMT
  host: docs.bigeye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: app.bigeye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bigeye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigeye, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bigeye
provider_slug: bigeye
slug: bigeye-domain-security
source_filename: bigeye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bigeye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 08:44:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.bigeye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 04:51:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.bigeye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bigeye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/security/bigeye-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Observability
- Data Quality
- Data Lineage
- Data Governance
- Metadata Management
- Data Catalog
- Sensitive Data Discovery
- Monitoring
- Analytics
- AI Trust
- Snowflake
- Databricks
---
