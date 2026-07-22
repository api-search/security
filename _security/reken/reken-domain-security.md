---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reken.ai
  spf: true
hosts:
- cert_expires: Sep 10 02:20:09 2026 GMT
  host: reken.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reken Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reken, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reken
provider_slug: reken
slug: reken-domain-security
source_filename: reken-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reken.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 02:20:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: reken.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reken/refs/heads/main/security/reken-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Security
- Cybersecurity
- Fraud Detection
- Anti-Phishing
- Deepfakes
- Trust and Safety
- On-Device AI
---
