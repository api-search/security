---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: duckdb.org
  spf: true
hosts:
- cert_expires: Sep  6 19:59:58 2026 GMT
  host: duckdb.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duckdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DuckDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DuckDB
provider_slug: duckdb
slug: duckdb-domain-security
source_filename: duckdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duckdb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:59:58 2026 GMT\n  hsts: false\ndomains:\n- domain: duckdb.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duckdb/refs/heads/main/security/duckdb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Database
- Analytics
- OLAP
- Embedded
- Open Source
---
