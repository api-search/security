---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pleaseassistme.com
  spf: true
hosts:
- cert_expires: Sep 29 20:14:58 2026 GMT
  host: pleaseassistme.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Please Assist Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Please Assist Me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Please Assist Me
provider_slug: please-assist-me
slug: please-assist-me-domain-security
source_filename: please-assist-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pleaseassistme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pleaseassistme.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/please-assist-me/refs/heads/main/security/please-assist-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Home Services
- Cleaning
- Errands
- Property Technology
- Consumer
- Apartment
---
