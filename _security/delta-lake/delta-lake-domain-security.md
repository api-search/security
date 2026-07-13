---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: delta.io
  spf: false
hosts:
- cert_expires: Sep 14 13:09:03 2026 GMT
  host: delta.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 13:09:03 2026 GMT
  host: docs.delta.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Delta Lake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delta Lake, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Delta Lake
provider_slug: delta-lake
slug: delta-lake-domain-security
source_filename: delta-lake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:09:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.delta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:09:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: delta.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delta-lake/refs/heads/main/security/delta-lake-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Data
- Data Lake
- Lakehouse
- Linux Foundation
- Open Source
- Storage
- Streaming
---
