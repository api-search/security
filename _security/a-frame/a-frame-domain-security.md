---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aframebrands.com
  spf: true
hosts:
- cert_expires: Oct 14 13:16:11 2026 GMT
  host: aframebrands.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: A Frame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A-Frame, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: A-Frame
provider_slug: a-frame
slug: a-frame-domain-security
source_filename: a-frame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aframebrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 13:16:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aframebrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a-frame/refs/heads/main/security/a-frame-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Consumer Packaged Goods
- Personal Care
- Beauty
- Brand Incubator
- Retail
- Venture Backed
---
