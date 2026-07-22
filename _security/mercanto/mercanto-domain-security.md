---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mercanto.mx
  spf: true
hosts:
- cert_expires: Sep 25 16:29:47 2026 GMT
  host: mercanto.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercanto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercanto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mercanto
provider_slug: mercanto
slug: mercanto-domain-security
source_filename: mercanto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mercanto.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:29:47 2026 GMT\n  hsts: false\ndomains:\n- domain: mercanto.mx\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercanto/refs/heads/main/security/mercanto-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Commerce
- Marketplace
- Wholesale
- Food and Beverage
- Restaurants
- B2B
- Supply Chain
- Grocery
- Mexico
---
