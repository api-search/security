---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: upciti.com
  spf: true
hosts:
- cert_expires: Aug 25 23:03:50 2026 GMT
  host: upciti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upciti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upciti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Upciti
provider_slug: upciti
slug: upciti-domain-security
source_filename: upciti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upciti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:03:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upciti.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upciti/refs/heads/main/security/upciti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Cities
- IoT
- Sensors
- Urban Data
- Computer Vision
- Environmental Monitoring
- Parking
- Mobility
- Air Quality
---
