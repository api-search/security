---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ev3.xyz
  spf: true
hosts:
- cert_expires: Aug 27 09:26:21 2026 GMT
  host: ev3.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ev3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EV3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EV3
provider_slug: ev3
slug: ev3-domain-security
source_filename: ev3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ev3.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:26:21 2026 GMT\n  hsts: false\ndomains:\n- domain: ev3.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ev3/refs/heads/main/security/ev3-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- Venture Capital
- Blockchain
- DePIN
- Investment
- Web3
---
