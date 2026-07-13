---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: motherduck.com
  spf: true
hosts:
- cert_expires: Sep 21 23:28:34 2026 GMT
  host: motherduck.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motherduck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MotherDuck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MotherDuck
provider_slug: motherduck
slug: motherduck-domain-security
source_filename: motherduck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motherduck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:28:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: motherduck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motherduck/refs/heads/main/security/motherduck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Warehouse
- Serverless
- DuckDB
- SQL
- Analytics
---
