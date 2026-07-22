---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quantums.com.sa
  spf: false
hosts:
- cert_expires: Oct  3 06:11:41 2026 GMT
  host: quantums.com.sa
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Quantum
provider_slug: quantum
slug: quantum-domain-security
source_filename: quantum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quantums.com.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:11:41 2026 GMT\n  hsts: false\ndomains:\n- domain: quantums.com.sa\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantum/refs/heads/main/security/quantum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- AdTech
- Marketing
- Programmatic
- Omnichannel
- Retail Media
- Saudi Arabia
---
