---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: toyota-global.com
  spf: false
hosts:
- cert_expires: Sep 30 14:59:59 2026 GMT
  host: www.toyota-global.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Toyota Motor Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toyota Motor Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Toyota Motor Corporation
provider_slug: toyota-motor-corporation
slug: toyota-motor-corporation-domain-security
source_filename: toyota-motor-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.toyota-global.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 14:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: toyota-global.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toyota-motor-corporation/refs/heads/main/security/toyota-motor-corporation-domain-security.yml
summary_line: TLSv1.2
tags:
- Automobiles
- Manufacturing
- Electric Vehicles
- Hybrid
---
