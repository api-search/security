---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swoop.com.ng
  spf: true
hosts:
- cert_expires: Sep 23 16:44:56 2026 GMT
  host: www.swoop.com.ng
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swoop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swoop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swoop
provider_slug: swoop
slug: swoop-domain-security
source_filename: swoop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swoop.com.ng\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:44:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swoop.com.ng\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swoop/refs/heads/main/security/swoop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food Delivery
- E-Commerce
- Payments
- Africa
- Nigeria
- Super App
- Mobile App
- Consumer
---
