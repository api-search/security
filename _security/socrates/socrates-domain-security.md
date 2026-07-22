---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: socrates.ai
  spf: true
hosts:
- cert_expires: Oct  1 15:51:47 2026 GMT
  host: socrates.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Socrates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Socrates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Socrates
provider_slug: socrates
slug: socrates-domain-security
source_filename: socrates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: socrates.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:51:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: socrates.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socrates/refs/heads/main/security/socrates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Acquired
- AI Assistant
- Employee Experience
- Conversational AI
- Workplace
---
