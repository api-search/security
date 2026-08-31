---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sonatus.com
  spf: true
hosts:
- cert_expires: Oct 16 03:20:21 2026 GMT
  host: www.sonatus.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonatus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonatus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sonatus
provider_slug: sonatus
slug: sonatus-domain-security
source_filename: sonatus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonatus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:20:21 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: sonatus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonatus/refs/heads/main/security/sonatus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Software Defined Vehicle
- Vehicle Data
- Connected Vehicles
- Automotive Software
- Edge AI
- Telematics
- Embedded Software
- Artificial Intelligence
---
