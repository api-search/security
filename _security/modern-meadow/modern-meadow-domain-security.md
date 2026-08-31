---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modernmeadow.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: innovera-world.com
  spf: false
hosts:
- cert_expires: Oct  5 19:13:45 2026 GMT
  host: modernmeadow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 02:42:45 2026 GMT
  host: innovera-world.com
  hsts: false
  https: true
  note: Product site; most modernmeadow.com paths 301 here.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modern Meadow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modern Meadow, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Modern Meadow
provider_slug: modern-meadow
slug: modern-meadow-domain-security
source_filename: modern-meadow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modernmeadow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:13:45 2026 GMT\n  hsts: false\n- host: innovera-world.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 02:42:45 2026 GMT\n  hsts: false\n  note: Product site; most modernmeadow.com paths 301 here.\ndomains:\n- domain: modernmeadow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: innovera-world.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nnotes:\n- No /.well-known/security.txt on either host (404).\n- No CAA records and no DNSSEC on either domain; no HSTS header on either host.\n- innovera-world.com publishes neither SPF nor DMARC, so the product domain is unprotected\n  against email spoofing while the corporate domain is at p=quarantine.\n- legacy.modernmeadow.com (the /careers redirect target)\
  \ fails the TLS handshake\n  (tlsv1 alert internal error), so the careers link off modernmeadow.com is broken.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modern-meadow/refs/heads/main/security/modern-meadow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Materials
- Biotechnology
- Synthetic Biology
- Biofabrication
- Sustainability
- Advanced Materials
- Fashion
- Footwear
- Automotive
- Interiors
- Manufacturing
- New Jersey
---
