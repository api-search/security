---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airwave.us
  spf: false
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: www.airwave.us
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airwave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Airwave
provider_slug: airwave
slug: airwave-domain-security
source_filename: airwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airwave.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: airwave.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airwave/refs/heads/main/security/airwave-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Field Service
- Smart Glasses
- Wearables
- Computer-Vision
- Industrial
- AI Assistant
- Inspection Reports
- Safety
---
