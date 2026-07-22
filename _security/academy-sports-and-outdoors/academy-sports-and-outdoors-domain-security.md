---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: academy.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.academy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Academy Sports And Outdoors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Academy Sports and Outdoors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Academy Sports and Outdoors
provider_slug: academy-sports-and-outdoors
slug: academy-sports-and-outdoors-domain-security
source_filename: academy-sports-and-outdoors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.academy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: academy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/academy-sports-and-outdoors/refs/heads/main/security/academy-sports-and-outdoors-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 500
- Retail
- Sporting Goods
- Outdoor Recreation
- E-Commerce
---
