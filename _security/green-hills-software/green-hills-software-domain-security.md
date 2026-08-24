---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ghs.com
  spf: true
hosts:
- cert_expires: Oct 16 08:33:46 2026 GMT
  host: www.ghs.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Hills Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Hills Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Green Hills Software
provider_slug: green-hills-software
slug: green-hills-software-domain-security
source_filename: green-hills-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ghs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 08:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: ghs.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-hills-software/refs/heads/main/security/green-hills-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Embedded Systems
- Real-Time Operating Systems
- RTOS
- Compilers
- Developer Tools
- Debugging
- Virtualization
- Safety Critical
- Automotive
- Aerospace and Defense
- Cybersecurity
---
