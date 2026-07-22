---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mayvenn.com
  spf: true
hosts:
- cert_expires: Sep 18 10:39:33 2026 GMT
  host: shop.mayvenn.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mayvenn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mayvenn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mayvenn
provider_slug: mayvenn
slug: mayvenn-domain-security
source_filename: mayvenn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shop.mayvenn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:39:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: mayvenn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mayvenn/refs/heads/main/security/mayvenn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beauty
- Hair Care
- E-Commerce
- Retail
- Consumer Goods
- Cosmetics
---
