---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rivosinc.com
  spf: true
hosts:
- cert_expires: Sep 25 19:36:49 2026 GMT
  host: rivosinc.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rivos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rivos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rivos
provider_slug: rivos
slug: rivos-domain-security
source_filename: rivos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rivosinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:36:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: rivosinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rivos/refs/heads/main/security/rivos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Hardware
- RISC-V
- GPU
- Accelerator
- Silicon
- Stealth
- Datacenter
- Acquired
---
