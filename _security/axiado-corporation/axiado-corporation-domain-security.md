---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: axiado.com
  spf: true
hosts:
- cert_expires: Sep 16 20:20:00 2026 GMT
  host: axiado.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 04:26:23 2026 GMT
  host: devhub.axiado.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axiado Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiado Corporation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Axiado Corporation
provider_slug: axiado-corporation
slug: axiado-corporation-domain-security
source_filename: axiado-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axiado.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:20:00 2026 GMT\n  hsts: false\n- host: devhub.axiado.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:26:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axiado.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiado-corporation/refs/heads/main/security/axiado-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Semiconductors
- Hardware Security
- Platform Security
- Data-Center
- Cybersecurity
- Baseboard Management Controller
- Root of Trust
- Firmware
- Embedded
- Cryptography
- AI Infrastructure
- Trusted Computing
- OpenBMC
- SDK
---
