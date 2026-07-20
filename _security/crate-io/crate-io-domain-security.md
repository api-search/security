---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cratedb.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cratedb.cloud
  spf: true
hosts:
- cert_expires: Aug 17 06:48:30 2026 GMT
  host: cratedb.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 13:25:41 2026 GMT
  host: console.cratedb.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crate Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crate Io, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crate Io
provider_slug: crate-io
slug: crate-io-domain-security
source_filename: crate-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cratedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 06:48:30 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: console.cratedb.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:25:41 2026 GMT\n  hsts: false\ndomains:\n- domain: cratedb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cratedb.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crate-io/refs/heads/main/security/crate-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Database
- SQL
- Distributed Database
- Analytics
- Time Series
- Vector Database
- IoT
- Cloud
- Developer Tools
---
