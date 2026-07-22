---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: itemku.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fivejack.com
  spf: true
hosts:
- cert_expires: Aug 25 11:37:01 2026 GMT
  host: www.itemku.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 09:09:20 2026 GMT
  host: fivejack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Five Jack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Five Jack, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Five Jack
provider_slug: five-jack
slug: five-jack-domain-security
source_filename: five-jack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.itemku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:37:01 2026 GMT\n  hsts: false\n- host: fivejack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 09:09:20 2026 GMT\n  hsts: false\ndomains:\n- domain: itemku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fivejack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/five-jack/refs/heads/main/security/five-jack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Gaming
- Digital Goods
- Ecommerce
- Indonesia
- Game Top-Up
- Consumer
---
