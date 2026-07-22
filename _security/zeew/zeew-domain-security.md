---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zeew.eu
  spf: true
hosts:
- cert_expires: Oct  6 22:48:16 2026 GMT
  host: zeew.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeew, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zeew
provider_slug: zeew
slug: zeew-domain-security
source_filename: zeew-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeew.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:48:16 2026 GMT\n  hsts: false\ndomains:\n- domain: zeew.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeew/refs/heads/main/security/zeew-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Delivery
- On-Demand
- Food Delivery
- Logistics
- White-Label
- SaaS
- Marketplace
---
