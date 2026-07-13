---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: playerdb.co
  spf: false
hosts:
- cert_expires: Sep  3 23:50:34 2026 GMT
  host: playerdb.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playerdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlayerDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: PlayerDB
provider_slug: playerdb
slug: playerdb-domain-security
source_filename: playerdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playerdb.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:50:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: playerdb.co\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playerdb/refs/heads/main/security/playerdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Games And Comics
- Public APIs
---
