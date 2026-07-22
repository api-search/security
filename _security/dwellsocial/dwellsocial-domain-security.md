---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dwellsocial.com
  spf: true
hosts:
- cert_expires: Oct  1 23:13:18 2026 GMT
  host: dwellsocial.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dwellsocial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DwellSocial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DwellSocial
provider_slug: dwellsocial
slug: dwellsocial-domain-security
source_filename: dwellsocial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dwellsocial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:13:18 2026 GMT\n  hsts: false\ndomains:\n- domain: dwellsocial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dwellsocial/refs/heads/main/security/dwellsocial-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food & Drink
- Food Delivery
- Restaurants
- Community
- Local Commerce
- Consumer
- Techstars
---
