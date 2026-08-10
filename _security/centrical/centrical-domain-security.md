---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centrical.com
  spf: true
hosts:
- cert_expires: Sep 30 12:47:49 2026 GMT
  host: centrical.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Centrical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centrical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Centrical
provider_slug: centrical
slug: centrical-domain-security
source_filename: centrical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centrical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:47:49 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: centrical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrical/refs/heads/main/security/centrical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Engagement
- Performance Management
- Gamification
- Microlearning
- Contact Center
- Workforce Engagement Management
- Coaching
- Quality Management
- Human Resources
- SaaS
---
