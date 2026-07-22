---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: i-brain.tech
  spf: true
hosts:
- cert_expires: Sep 11 04:50:36 2026 GMT
  host: i-brain.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: I Brain Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for i-Brain Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: i-Brain Tech
provider_slug: i-brain-tech
slug: i-brain-tech-domain-security
source_filename: i-brain-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: i-brain.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:50:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: i-brain.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/i-brain-tech/refs/heads/main/security/i-brain-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Sports
- Neuroscience
- Neurofeedback
- Health
- Rehabilitation
- Cognitive Training
- Athletics
---
