---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rethinkdb.com
  spf: true
hosts:
- cert_expires: Oct  7 14:13:48 2026 GMT
  host: rethinkdb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rethinkdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RethinkDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RethinkDB
provider_slug: rethinkdb
slug: rethinkdb-domain-security
source_filename: rethinkdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rethinkdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rethinkdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rethinkdb/refs/heads/main/security/rethinkdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- NoSQL
- Document Database
- Real-Time
- Open Source
- Change Feeds
- ReQL
---
