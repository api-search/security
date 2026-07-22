---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: airspace-intelligence.com
  spf: true
hosts:
- cert_expires: Sep 26 04:59:12 2026 GMT
  host: www.airspace-intelligence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Air Space Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Air Space Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Air Space Intelligence
provider_slug: air-space-intelligence
slug: air-space-intelligence-domain-security
source_filename: air-space-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airspace-intelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:59:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airspace-intelligence.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/air-space-intelligence/refs/heads/main/security/air-space-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Aviation
- Aerospace
- Artificial Intelligence
- Defense
- Air Traffic Management
- Optimization
- Logistics
- Situational Awareness
---
