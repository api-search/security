---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fruitist.com
  spf: true
hosts:
- cert_expires: Nov  5 23:55:45 2026 GMT
  host: www.fruitist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 22:18:01 2026 GMT
  host: shop.fruitist.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agrovision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agrovision, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agrovision
provider_slug: agrovision
slug: agrovision-domain-security
source_filename: agrovision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fruitist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:55:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shop.fruitist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 22:18:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: fruitist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrovision/refs/heads/main/security/agrovision-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Food and Beverage
- Consumer Packaged Goods
- AgTech
- E-Commerce
- Retail
- Supply Chain
- Agentic Commerce
- Universal Commerce Protocol
---
