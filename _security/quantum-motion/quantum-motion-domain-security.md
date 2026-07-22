---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quantummotion.tech
  spf: true
hosts:
- cert_expires: Oct  2 12:50:55 2026 GMT
  host: quantummotion.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantum Motion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantum Motion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quantum Motion
provider_slug: quantum-motion
slug: quantum-motion-domain-security
source_filename: quantum-motion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quantummotion.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:50:55 2026 GMT\n  hsts: false\ndomains:\n- domain: quantummotion.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantum-motion/refs/heads/main/security/quantum-motion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Quantum Computing
- Deep Tech
- Hardware
- Semiconductors
- Research
---
