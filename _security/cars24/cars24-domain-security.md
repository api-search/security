---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cars24.com
  spf: true
hosts:
- cert_expires: Sep 30 02:59:14 2026 GMT
  host: cars24.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cars24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cars24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cars24
provider_slug: cars24
slug: cars24-domain-security
source_filename: cars24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cars24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:59:14 2026 GMT\n  hsts: false\ndomains:\n- domain: cars24.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cars24/refs/heads/main/security/cars24-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Used Cars
- Marketplace
- Auto Finance
- Vehicle Inspection
- Fintech
- India
- E-Commerce
---
