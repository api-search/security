---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brooklyndumplingshop.com
  spf: true
hosts:
- cert_expires: Dec  1 19:32:24 2026 GMT
  host: www.brooklyndumplingshop.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brooklyn Dumpling Shop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brooklyn Dumpling Shop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brooklyn Dumpling Shop
provider_slug: brooklyn-dumpling-shop
slug: brooklyn-dumpling-shop-domain-security
source_filename: brooklyn-dumpling-shop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brooklyndumplingshop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 19:32:24 2026 GMT\n  hsts: false\ndomains:\n- domain: brooklyndumplingshop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brooklyn-dumpling-shop/refs/heads/main/security/brooklyn-dumpling-shop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurant
- Fast Casual
- Asian Fusion
- Dumplings
---
