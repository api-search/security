---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cartrawler.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.cartrawler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cartrawler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cartrawler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cartrawler
provider_slug: cartrawler
slug: cartrawler-domain-security
source_filename: cartrawler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cartrawler.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cartrawler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartrawler/refs/heads/main/security/cartrawler-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Travel
- Car Rental
- Mobility
- Ground Transport
- Insurtech
- Travel Technology
- B2B
- Marketplace
---
