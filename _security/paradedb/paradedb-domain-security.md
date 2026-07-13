---
api_specs:
- filename: paradedb-openapi.yml
  format: yaml
  label: ParadeDB pg_search (Full-Text Search)
  slug: pg_search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradedb/refs/heads/main/openapi/paradedb-openapi.yml
- filename: paradedb-openapi.yml
  format: yaml
  label: ParadeDB Analytics (pg_analytics)
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradedb/refs/heads/main/openapi/paradedb-openapi.yml
- filename: paradedb-openapi.yml
  format: yaml
  label: ParadeDB Postgres SQL Interface
  slug: postgres-sql-interface
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradedb/refs/heads/main/openapi/paradedb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paradedb.com
  spf: true
hosts:
- cert_expires: Aug 15 14:31:05 2026 GMT
  host: www.paradedb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:17:47 2026 GMT
  host: docs.paradedb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paradedb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParadeDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ParadeDB
provider_slug: paradedb
slug: paradedb-domain-security
source_filename: paradedb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paradedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 14:31:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.paradedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:17:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: paradedb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradedb/refs/heads/main/security/paradedb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Full-Text Search
- Analytics
- PostgreSQL
- Database
- Elasticsearch Alternative
---
