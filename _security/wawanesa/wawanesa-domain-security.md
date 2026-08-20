---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wawanesa.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: www.wawanesa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wawanesa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wawanesa Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wawanesa Insurance
provider_slug: wawanesa
slug: wawanesa-domain-security
source_filename: wawanesa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wawanesa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wawanesa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wawanesa/refs/heads/main/security/wawanesa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Property and Casualty
- Carrier
- Mutual Insurer
- Brokers
- Commercial Lines
- Personal Lines
- Underwriting
- Claims
- Policy Administration
- CSIO
- Partner Gated
---
