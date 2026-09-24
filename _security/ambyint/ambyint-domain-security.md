---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ambyint.com
  spf: true
hosts:
- cert_expires: Nov 19 10:21:50 2026 GMT
  host: www.ambyint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ambyint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambyint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ambyint
provider_slug: ambyint
slug: ambyint-domain-security
source_filename: ambyint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ambyint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 10:21:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ambyint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambyint/refs/heads/main/security/ambyint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Production Optimization
- Artificial Lift
- Oil & Gas
- AI
- Autonomous Setpoint Management
- Anomaly Detection
- Analytics
---
