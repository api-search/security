---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bevspot.com
  spf: true
hosts:
- cert_expires: Oct 11 03:26:35 2026 GMT
  host: bevspot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bevspot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BevSpot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BevSpot
provider_slug: bevspot
slug: bevspot-domain-security
source_filename: bevspot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bevspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 03:26:35 2026 GMT\n  hsts: false\ndomains:\n- domain: bevspot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bevspot/refs/heads/main/security/bevspot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Apps
- Restaurant
- Hospitality
- Inventory Management
- Food And Beverage
- Point Of Sale
- Analytics
- SaaS
---
