---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: m7health.com
  spf: true
hosts:
- cert_expires: Sep  4 15:29:26 2026 GMT
  host: www.m7health.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: M7 Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M7 Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: M7 Health
provider_slug: m7-health
slug: m7-health-domain-security
source_filename: m7-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.m7health.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:29:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: m7health.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m7-health/refs/heads/main/security/m7-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Nurse Scheduling
- Workforce Management
- Labor Optimization
- Staffing
- Artificial Intelligence
---
