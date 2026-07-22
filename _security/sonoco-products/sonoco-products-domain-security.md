---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sonoco.com
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.sonoco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonoco Products Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonoco Products, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sonoco Products
provider_slug: sonoco-products
slug: sonoco-products-domain-security
source_filename: sonoco-products-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonoco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sonoco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonoco-products/refs/heads/main/security/sonoco-products-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Packaging
- Manufacturing
- Consumer Goods
- Industrial
- Sustainability
- Fortune 500
---
