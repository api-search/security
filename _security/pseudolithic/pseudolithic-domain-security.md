---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pseudolithic.com
  spf: true
hosts:
- cert_expires: Sep 11 15:34:27 2026 GMT
  host: pseudolithic.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pseudolithic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pseudolithic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pseudolithic
provider_slug: pseudolithic
slug: pseudolithic-domain-security
source_filename: pseudolithic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pseudolithic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:34:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: pseudolithic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pseudolithic/refs/heads/main/security/pseudolithic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Semiconductors
- Hardware
- RFIC
- Radio Frequency
- Heterogeneous Integration
- Chiplets
- Power Amplifiers
---
