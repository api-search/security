---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: butternutbox.com
  spf: true
hosts:
- cert_expires: Oct 22 17:53:09 2026 GMT
  host: butternutbox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Butternut Box Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Butternut Box, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Butternut Box
provider_slug: butternut-box
slug: butternut-box-domain-security
source_filename: butternut-box-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: butternutbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 17:53:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: butternutbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butternut-box/refs/heads/main/security/butternut-box-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pet Care
- Pet Food
- Direct to Consumer
- Subscription
- E-Commerce
- Food and Beverage
- Consumer Goods
- United Kingdom
---
