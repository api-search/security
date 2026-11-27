---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parkgraph.com
  spf: false
hosts:
- cert_expires: Jan  2 05:42:54 2027 GMT
  host: parkgraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Park Graph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Park Graph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Park Graph
provider_slug: parkgraph-com
slug: parkgraph-com-domain-security
source_filename: parkgraph-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parkgraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 05:42:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: parkgraph.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/parkgraph-com/security/parkgraph-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Parking
- QR Payments
- Parking Management
- Contactless Payments
- Lot Owners
- Revenue Share
---
