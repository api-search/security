---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: catchbackcards.com
  spf: true
hosts:
- cert_expires: Sep 20 00:09:22 2026 GMT
  host: catchbackcards.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catchback Cards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catchback Cards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Catchback Cards
provider_slug: catchback-cards
slug: catchback-cards-domain-security
source_filename: catchback-cards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catchbackcards.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:09:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: catchbackcards.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catchback-cards/refs/heads/main/security/catchback-cards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trading Cards
- Collectibles
- Marketplace
- Consumer
- Mobile
- Payments
- Y Combinator
---
