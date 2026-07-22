---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fullcourt.co
  spf: true
hosts:
- cert_expires: Oct 14 20:31:47 2026 GMT
  host: fullcourt.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Japan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fullcourt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fullcourt
provider_slug: japan
slug: japan-domain-security
source_filename: japan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fullcourt.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:31:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fullcourt.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/japan/refs/heads/main/security/japan-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Customer Support
- Helpdesk
- Ecommerce
- Shopify
- DTC
- SaaS
---
