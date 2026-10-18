---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orioledb.com
  spf: false
hosts:
- cert_expires: Nov 22 04:14:20 2026 GMT
  host: www.orioledb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orioledb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OrioleDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OrioleDB
provider_slug: orioledb
slug: orioledb-domain-security
source_filename: orioledb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orioledb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 04:14:20 2026 GMT\n  hsts: false\ndomains:\n- domain: orioledb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orioledb/refs/heads/main/security/orioledb-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Database
- PostgreSQL
- Storage Engines
- Open Source
- Extensions
---
