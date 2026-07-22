---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mensabrands.com
  spf: true
hosts:
- cert_expires: Oct 11 15:38:57 2026 GMT
  host: mensabrands.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mensa Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mensa Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mensa Brands
provider_slug: mensa-brands
slug: mensa-brands-domain-security
source_filename: mensa-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mensabrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 15:38:57 2026 GMT\n  hsts: false\ndomains:\n- domain: mensabrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mensa-brands/refs/heads/main/security/mensa-brands-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Ecommerce
- Retail
- Fashion
- Beauty
- House of Brands
- D2C
---
