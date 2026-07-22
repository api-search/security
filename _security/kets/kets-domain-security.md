---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kets-quantum.com
  spf: true
hosts:
- cert_expires: Oct  8 18:32:08 2026 GMT
  host: kets-quantum.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kets
provider_slug: kets
slug: kets-domain-security
source_filename: kets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kets-quantum.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 18:32:08 2026 GMT\n  hsts: null\ndomains:\n- domain: kets-quantum.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kets/refs/heads/main/security/kets-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Quantum Security
- Cybersecurity
- Quantum Key Distribution
- Quantum Random Number Generator
- Post-Quantum Cryptography
- Encryption
- Photonics
- Hardware
- Deep Tech
---
