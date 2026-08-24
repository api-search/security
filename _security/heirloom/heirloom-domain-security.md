---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: heirloomcarbon.com
  spf: true
hosts:
- cert_expires: Nov  7 09:12:54 2026 GMT
  host: www.heirloomcarbon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heirloom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heirloom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Heirloom
provider_slug: heirloom
slug: heirloom-domain-security
source_filename: heirloom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heirloomcarbon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 09:12:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heirloomcarbon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heirloom/refs/heads/main/security/heirloom-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Carbon Removal
- Direct Air Capture
- Climate Technology
- Carbon Credits
- Sustainability
- Energy
- Climate
---
