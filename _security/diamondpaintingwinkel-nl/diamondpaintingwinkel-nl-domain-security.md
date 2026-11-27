---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: diamondpaintingwinkel.nl
  spf: true
hosts:
- cert_expires: Jan 16 17:54:21 2027 GMT
  host: diamondpaintingwinkel.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DiamondPaintingWinkel.nl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DiamondPaintingWinkel.nl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DiamondPaintingWinkel.nl
provider_slug: diamondpaintingwinkel-nl
slug: diamondpaintingwinkel-nl-domain-security
source_filename: diamondpaintingwinkel-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diamondpaintingwinkel.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 17:54:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: diamondpaintingwinkel.nl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/diamondpaintingwinkel-nl/security/diamondpaintingwinkel-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Diamond Painting
- E-Commerce
- Arts and Crafts
- Netherlands
- Retail
---
