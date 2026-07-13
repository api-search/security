---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tigerbeetle.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: tigerbeetle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 13:27:18 2026 GMT
  host: docs.tigerbeetle.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tigerbeetle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TigerBeetle, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TigerBeetle
provider_slug: tigerbeetle
slug: tigerbeetle-domain-security
source_filename: tigerbeetle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tigerbeetle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tigerbeetle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:27:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: tigerbeetle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigerbeetle/refs/heads/main/security/tigerbeetle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Accounting
- Transactions
- Database
- Double-Entry
- Ledger
- OLTP
- Distributed
- Open Source
- Binary Protocol
---
