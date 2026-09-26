---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: angstromsports.com
  spf: true
hosts:
- cert_expires: Nov 22 14:14:13 2026 GMT
  host: angstromsports.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Angstrom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angstrom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Angstrom
provider_slug: angstrom
slug: angstrom-domain-security
source_filename: angstrom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: angstromsports.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 14:14:13 2026 GMT\n  hsts: false\ndomains:\n- domain: angstromsports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angstrom/refs/heads/main/security/angstrom-domain-security.yml
summary_line: TLSv1.2
tags:
- Sports
- Analytics
- Forecasting
- Betting
- Data
---
