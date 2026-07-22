---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dastechnology.com
  spf: true
hosts:
- cert_expires: Oct 14 22:43:32 2026 GMT
  host: www.dastechnology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Das Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DAS Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DAS Technology
provider_slug: das-technology
slug: das-technology-domain-security
source_filename: das-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dastechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:43:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dastechnology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/das-technology/refs/heads/main/security/das-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- Automotive
- Automotive Retail
- Marketing
- Customer Data Platform
- Advertising
- Reputation Management
---
