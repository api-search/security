---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: humansecurity.com
  spf: true
hosts:
- cert_expires: Sep 22 15:15:04 2026 GMT
  host: www.humansecurity.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 17:02:34 2026 GMT
  host: docs.humansecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Apr  7 23:59:59 2027 GMT
  host: console.humansecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Perimeterx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PerimeterX (HUMAN Security), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PerimeterX (HUMAN Security)
provider_slug: perimeterx
slug: perimeterx-domain-security
source_filename: perimeterx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.humansecurity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 15:15:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.humansecurity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 17:02:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: console.humansecurity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humansecurity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perimeterx/refs/heads/main/security/perimeterx-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Bot Mitigation
- Application Security
- Fraud Prevention
- Ad Fraud
- Account Takeover
- Agentic AI
- Cybersecurity
- API
---
