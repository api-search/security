---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doctorly.de
  spf: true
hosts:
- cert_expires: Aug 24 01:08:25 2026 GMT
  host: doctorly.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doctorly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doctorly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Doctorly
provider_slug: doctorly
slug: doctorly-domain-security
source_filename: doctorly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doctorly.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:08:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doctorly.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctorly/refs/heads/main/security/doctorly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health IT
- Practice Management
- Medical Software
- SaaS
- Germany
- Digital Health
---
