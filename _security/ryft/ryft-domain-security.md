---
api_specs:
- filename: ryft-ingest-openapi.yml
  format: yaml
  label: Ryft Ingest API
  slug: ryft-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryft/refs/heads/main/openapi/ryft-ingest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ryft.io
  spf: true
hosts:
- cert_expires: Sep 22 18:00:04 2026 GMT
  host: www.ryft.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 09:28:37 2026 GMT
  host: docs.ryft.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: ingest.ryft.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ryft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ryft, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ryft
provider_slug: ryft
slug: ryft-domain-security
source_filename: ryft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ryft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:00:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ryft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:28:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ingest.ryft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ryft.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryft/refs/heads/main/security/ryft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Data Lake
- Lakehouse
- Apache Iceberg
- Data Management
- Analytics
- Query Optimization
- AI
- MCP
---
