---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liquidinstruments.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: liquidinstruments.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: apis.liquidinstruments.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: auth.liquidinstruments.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liquid Instruments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquid Instruments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liquid Instruments
provider_slug: liquid-instruments
slug: liquid-instruments-domain-security
source_filename: liquid-instruments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liquidinstruments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: apis.liquidinstruments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\n- host: auth.liquidinstruments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: liquidinstruments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-instruments/refs/heads/main/security/liquid-instruments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Test and Measurement
- Instrumentation
- Hardware
- Oscilloscope
- Spectrum Analyzer
- Data Acquisition
- FPGA
- Photonics
- Scientific Instruments
- Electronics
- Laboratory
---
