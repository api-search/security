---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: isaacinstruments.com
  spf: true
hosts:
- cert_expires: Sep 14 15:38:45 2026 GMT
  host: www.isaacinstruments.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Isaac Instruments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ISAAC Instruments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ISAAC Instruments
provider_slug: isaac-instruments
slug: isaac-instruments-domain-security
source_filename: isaac-instruments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.isaacinstruments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:38:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: isaacinstruments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isaac-instruments/refs/heads/main/security/isaac-instruments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trucking
- Telematics
- ELD
- Fleet Management
- Hours of Service
- Compliance
- Transportation
- Partner API
---
