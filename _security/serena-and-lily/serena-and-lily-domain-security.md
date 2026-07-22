---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: serenaandlily.com
  spf: true
hosts:
- cert_expires: Sep 21 03:51:37 2026 GMT
  host: www.serenaandlily.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serena And Lily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serena & Lily, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Serena & Lily
provider_slug: serena-and-lily
slug: serena-and-lily-domain-security
source_filename: serena-and-lily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.serenaandlily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:51:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: serenaandlily.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serena-and-lily/refs/heads/main/security/serena-and-lily-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Home Furnishings
- Retail
- E-Commerce
- Interior Design
- Direct to Consumer
---
