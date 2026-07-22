---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: saucey.com
  spf: true
hosts:
- cert_expires: Oct  1 04:14:57 2026 GMT
  host: saucey.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Saucey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saucey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Saucey
provider_slug: saucey
slug: saucey-domain-security
source_filename: saucey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saucey.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 04:14:57 2026 GMT\n  hsts: false\ndomains:\n- domain: saucey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saucey/refs/heads/main/security/saucey-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Alcohol Delivery
- On-Demand Delivery
- E-Commerce
- Logistics
- Consumer
- Marketplace
---
