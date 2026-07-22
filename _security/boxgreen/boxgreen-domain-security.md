---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boxgreen.co
  spf: true
hosts:
- cert_expires: Sep  1 00:22:02 2026 GMT
  host: boxgreen.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boxgreen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoxGreen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BoxGreen
provider_slug: boxgreen
slug: boxgreen-domain-security
source_filename: boxgreen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boxgreen.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:22:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: boxgreen.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boxgreen/refs/heads/main/security/boxgreen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthy Snacks
- E-Commerce
- Consumer Packaged Goods
- Subscription
- Corporate Gifting
- Social Enterprise
- B Corporation
- Food and Beverage
- Singapore
---
