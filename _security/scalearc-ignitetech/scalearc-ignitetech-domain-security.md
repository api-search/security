---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: devgraph.com
  spf: true
hosts:
- cert_expires: Sep 11 05:23:24 2026 GMT
  host: www.devgraph.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalearc Ignitetech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScaleArc (IgniteTech), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ScaleArc (IgniteTech)
provider_slug: scalearc-ignitetech
slug: scalearc-ignitetech-domain-security
source_filename: scalearc-ignitetech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.devgraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:23:24 2026 GMT\n  hsts: false\ndomains:\n- domain: devgraph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalearc-ignitetech/refs/heads/main/security/scalearc-ignitetech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Infrastructure
- Database
- Load Balancing
- SQL Server
- MySQL
- High Availability
- Database Management
- Connection Pooling
---
