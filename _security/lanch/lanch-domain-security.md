---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lanch.com
  spf: true
hosts:
- cert_expires: Sep 29 22:27:56 2026 GMT
  host: www.lanch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lanch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lanch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lanch
provider_slug: lanch
slug: lanch-domain-security
source_filename: lanch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lanch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:27:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lanch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lanch/refs/heads/main/security/lanch-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Food
- Food Tech
- Food Delivery
- Restaurants
- Franchise
- Ghost Kitchen
- Creator Economy
- Germany
---
