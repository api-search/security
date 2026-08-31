---
api_specs:
- filename: tiledb-cloud-v1-openapi.yaml
  format: yaml
  label: TileDB Storage Platform API (v1)
  slug: tiledb-storage-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-cloud-v1-openapi.yaml
- filename: tiledb-cloud-v2-openapi.yaml
  format: yaml
  label: TileDB Storage Platform API (v2)
  slug: tiledb-storage-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-cloud-v2-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tiledb.com
  spf: true
hosts:
- cert_expires: Oct 16 04:13:57 2026 GMT
  host: www.tiledb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: documentation.cloud.tiledb.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 16 04:13:57 2026 GMT
  host: api.tiledb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiledb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TileDB, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TileDB
provider_slug: tiledb
slug: tiledb-domain-security
source_filename: tiledb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiledb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 04:13:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.cloud.tiledb.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: false\n- host: api.tiledb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 04:13:57 2026 GMT\n  hsts: null\ndomains:\n- domain: tiledb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/security/tiledb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Database
- Multimodal Data
- Life Sciences
- Genomics
- Single Cell
- Biomedical Imaging
- Vector Search
- Data Management
- Cloud Storage
- Analytics
- Machine-Learning
---
