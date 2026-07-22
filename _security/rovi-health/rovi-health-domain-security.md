---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rovi.health
  spf: true
hosts:
- cert_expires: Oct 14 04:14:54 2026 GMT
  host: www.rovi.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rovi Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rovi Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rovi Health
provider_slug: rovi-health
slug: rovi-health-domain-security
source_filename: rovi-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rovi.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 04:14:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rovi.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rovi-health/refs/heads/main/security/rovi-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Health Insurance
- Care Navigation
- Employer Benefits
- Telehealth
---
