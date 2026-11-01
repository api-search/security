---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zen-cart.com
  spf: true
hosts:
- cert_expires: Dec 12 23:24:18 2026 GMT
  host: zen-cart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zen Cart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zen Cart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zen Cart
provider_slug: zen-cart
slug: zen-cart-domain-security
source_filename: zen-cart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zen-cart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:24:18 2026 GMT\n  hsts: null\ndomains:\n- domain: zen-cart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/zen-cart/security/zen-cart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- e-commerce
- open-source
- php
- shopping-cart
- community
- platform
---
