---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: britesemi.com
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.britesemi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Britesemi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Britesemi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Britesemi
provider_slug: britesemi
slug: britesemi-domain-security
source_filename: britesemi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.britesemi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: britesemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/britesemi/refs/heads/main/security/britesemi-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Semiconductor
- ASIC
- Silicon IP
- Chip Design
- SoC
- Hardware
---
