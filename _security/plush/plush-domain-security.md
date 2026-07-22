---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plush.shop
  spf: true
hosts:
- cert_expires: Sep 29 23:58:07 2026 GMT
  host: www.plush.shop
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plush, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plush
provider_slug: plush
slug: plush-domain-security
source_filename: plush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plush.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:58:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: plush.shop\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plush/refs/heads/main/security/plush-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- Retail
- Ecommerce
- Artificial Intelligence
- Search
- Shopping
- Consumer
---
