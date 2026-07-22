---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: framesecurity.com
  spf: true
hosts:
- cert_expires: Oct  5 22:35:20 2026 GMT
  host: framesecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frame Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frame Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Frame Security
provider_slug: frame-security
slug: frame-security-domain-security
source_filename: frame-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: framesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:35:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: framesecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frame-security/refs/heads/main/security/frame-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Security Awareness
- Human Risk Management
- Phishing Simulation
- Deepfake Detection
- Cybersecurity Training
- Compliance
---
