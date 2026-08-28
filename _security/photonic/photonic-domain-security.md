---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: photonic.com
  spf: true
hosts:
- cert_expires: Oct 28 06:54:58 2026 GMT
  host: photonic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Photonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Photonic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Photonic
provider_slug: photonic
slug: photonic-domain-security
source_filename: photonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: photonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 06:54:58 2026 GMT\n  hsts: false\ndomains:\n- domain: photonic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photonic/refs/heads/main/security/photonic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Quantum Computing
- Quantum Networking
- Silicon Photonics
- Semiconductors
- Deep Tech
- Research
- Hardware
- Canada
---
