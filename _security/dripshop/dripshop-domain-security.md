---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dripshop.live
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: dripshop.live
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.dripshop.live
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: GraphQL API host (Cloudflare); observed via HTTP HEAD
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dripshop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dripshop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dripshop
provider_slug: dripshop
slug: dripshop-domain-security
source_filename: dripshop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dripshop.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dripshop.live\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  note: GraphQL API host (Cloudflare); observed via HTTP HEAD\ndomains:\n- domain: dripshop.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dripshop/refs/heads/main/security/dripshop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Live Shopping
- Collectibles
- Trading Cards
- Marketplace
- Ecommerce
- Auctions
- Live Streaming
- Payments
- GraphQL
---
