---
api_specs:
- filename: delta-lake-delta-sharing-protocol-openapi.yml
  format: yaml
  label: Delta Sharing Protocol
  slug: delta-sharing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-lake/refs/heads/main/openapi/delta-lake-delta-sharing-protocol-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: delta.io
  spf: false
hosts:
- cert_expires: Nov 13 12:16:33 2026 GMT
  host: delta.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 12:16:33 2026 GMT
  host: docs.delta.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: sharing.delta.io
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Delta Lake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delta Lake, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Delta Lake
provider_slug: delta-lake
slug: delta-lake-domain-security
source_filename: delta-lake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 12:16:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.delta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 12:16:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sharing.delta.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: delta.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delta-lake/refs/heads/main/security/delta-lake-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Data
- Data Lake
- Lakehouse
- Linux Foundation
- Open-Source
- Storage
- Streaming
---
