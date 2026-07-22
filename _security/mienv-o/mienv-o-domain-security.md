---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mienvio.mx
  spf: true
hosts:
- cert_expires: Oct 15 17:13:04 2026 GMT
  host: mienvio.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mienv O Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mienvío, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mienvío
provider_slug: mienv-o
slug: mienv-o-domain-security
source_filename: mienv-o-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mienvio.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 17:13:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mienvio.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mienv-o/refs/heads/main/security/mienv-o-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Shipping
- Logistics
- Multi-Carrier
- E-commerce
- Fulfillment
- Package Tracking
- Mexico
- Latin America
---
