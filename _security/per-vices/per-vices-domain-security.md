---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pervices.com
  spf: true
hosts:
- cert_expires: Sep 13 07:48:55 2026 GMT
  host: www.pervices.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Per Vices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Per Vices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Per Vices
provider_slug: per-vices
slug: per-vices-domain-security
source_filename: per-vices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pervices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:48:55 2026 GMT\n  hsts: false\ndomains:\n- domain: pervices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/per-vices/refs/heads/main/security/per-vices-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Software Defined Radio
- SDR
- Radio Frequency
- Wireless
- Hardware
- FPGA
- Telecommunications
- Embedded Systems
---
