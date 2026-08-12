---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coreshell.com
  spf: true
hosts:
- cert_expires: Sep 12 15:40:08 2026 GMT
  host: www.coreshell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coreshell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coreshell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coreshell
provider_slug: coreshell
slug: coreshell-domain-security
source_filename: coreshell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coreshell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:40:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coreshell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coreshell/refs/heads/main/security/coreshell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Batteries
- Energy Storage
- Electric Vehicles
- Advanced Materials
- Manufacturing
- Clean Energy
- Defense
---
