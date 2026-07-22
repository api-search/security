---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deporprive.mx
  spf: true
hosts:
- cert_expires: Sep  6 06:09:47 2026 GMT
  host: deporprive.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Deporpriv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeporPrivé, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DeporPrivé
provider_slug: deporpriv
slug: deporpriv-domain-security
source_filename: deporpriv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deporprive.mx\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 06:09:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deporprive.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deporpriv/refs/heads/main/security/deporpriv-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Retail
- Sports
- Mexico
- Flash Sales
- Consumer
---
