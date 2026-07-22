---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: post-quantum.com
  spf: false
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: post-quantum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Post Quantum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Post-Quantum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Post-Quantum
provider_slug: post-quantum
slug: post-quantum-domain-security
source_filename: post-quantum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: post-quantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: post-quantum.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/post-quantum/refs/heads/main/security/post-quantum-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Security
- Cybersecurity
- Quantum
- Post-Quantum Cryptography
- Cryptography
- Encryption
- VPN
- Identity
---
