---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haseelapp.com
  spf: true
hosts:
- cert_expires: Aug 28 09:04:21 2026 GMT
  host: haseelapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Haseel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haseel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Haseel
provider_slug: haseel
slug: haseel-domain-security
source_filename: haseel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haseelapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 09:04:21 2026 GMT\n  hsts: false\ndomains:\n- domain: haseelapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haseel/refs/heads/main/security/haseel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Grocery
- Food Delivery
- E-Commerce
- Mobile App
- Produce
- Agriculture Technology
- Last-Mile Delivery
- Saudi Arabia
---
