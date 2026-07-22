---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bravosierra.com
  spf: true
hosts:
- cert_expires: Aug 26 22:05:33 2026 GMT
  host: www.bravosierra.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bravo Sierra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bravo Sierra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bravo Sierra
provider_slug: bravo-sierra
slug: bravo-sierra-domain-security
source_filename: bravo-sierra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bravosierra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:05:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: bravosierra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bravo-sierra/refs/heads/main/security/bravo-sierra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Personal Care
- Consumer Packaged Goods
- E-Commerce
- Direct to Consumer
- Beauty and Grooming
- Military and Veterans
- Made in USA
- Shopify
---
