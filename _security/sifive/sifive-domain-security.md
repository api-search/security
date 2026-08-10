---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sifive.com
  spf: true
hosts:
- cert_expires: Oct  6 23:21:14 2026 GMT
  host: www.sifive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: scs.sifive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sifive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SiFive, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SiFive
provider_slug: sifive
slug: sifive-domain-security
source_filename: sifive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sifive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:21:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: scs.sifive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sifive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sifive/refs/heads/main/security/sifive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- RISC-V
- Processor IP
- Chip Design
- Embedded
- Hardware
- Developer Tools
- Electronic Design Automation
- OAuth
---
