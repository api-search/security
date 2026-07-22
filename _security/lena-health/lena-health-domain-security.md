---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lena.io
  spf: false
hosts:
- cert_expires: Sep 23 14:02:51 2026 GMT
  host: lena.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lena Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lena Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Lena Health
provider_slug: lena-health
slug: lena-health-domain-security
source_filename: lena-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lena.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lena.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lena-health/refs/heads/main/security/lena-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Care Coordination
- Care Navigation
- Artificial Intelligence
- Patient Engagement
- Chronic Care Management
- Health Plans
- Digital Health
- HIPAA
---
