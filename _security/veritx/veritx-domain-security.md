---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: veritx.com
  spf: true
hosts:
- cert_expires: Oct 11 14:45:41 2026 GMT
  host: www.veritx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veritx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VeriTX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VeriTX
provider_slug: veritx
slug: veritx-domain-security
source_filename: veritx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veritx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:45:41 2026 GMT\n  hsts: false\ndomains:\n- domain: veritx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritx/refs/heads/main/security/veritx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Blockchain
- Cybersecurity
- Data Security
- Post-Quantum Cryptography
- Supply Chain
- Aerospace
- Additive Manufacturing
- Provenance
- Defense
---
