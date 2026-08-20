---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bulletproof.com
  spf: true
hosts:
- cert_expires: Oct 28 02:46:37 2026 GMT
  host: www.bulletproof.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 22:34:01 2026 GMT
  host: shop.bulletproof.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bulletproof Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BulletProof, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BulletProof
provider_slug: bulletproof
slug: bulletproof-domain-security
source_filename: bulletproof-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bulletproof.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 02:46:37 2026 GMT\n  hsts: false\n- host: shop.bulletproof.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 22:34:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: bulletproof.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bulletproof/refs/heads/main/security/bulletproof-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- Health and Wellness
- Supplements
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
---
