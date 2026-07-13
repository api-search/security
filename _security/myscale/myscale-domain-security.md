---
api_specs:
- filename: myscale-openapi.yml
  format: yaml
  label: MyScale SQL Interface (ClickHouse HTTP)
  slug: myscale-sql-http-interface
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myscale/refs/heads/main/openapi/myscale-openapi.yml
- filename: myscale-openapi.yml
  format: yaml
  label: MyScale Vector Search (SQL)
  slug: myscale-vector-search-sql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myscale/refs/heads/main/openapi/myscale-openapi.yml
- filename: myscale-openapi.yml
  format: yaml
  label: MyScale Python SDK (clickhouse-connect)
  slug: myscale-python-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myscale/refs/heads/main/openapi/myscale-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: myscale.com
  spf: true
hosts:
- cert_expires: Sep 26 06:02:35 2026 GMT
  host: www.myscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 13:51:30 2026 GMT
  host: docs.myscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 08:58:50 2026 GMT
  host: myscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyScale, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MyScale
provider_slug: myscale
slug: myscale-domain-security
source_filename: myscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:02:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.myscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:51:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: myscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:58:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: myscale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myscale/refs/heads/main/security/myscale-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Vector Database
- SQL
- ClickHouse
- Vector Search
- Full-Text Search
- RAG
---
