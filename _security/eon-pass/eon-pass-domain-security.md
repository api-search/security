---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eonpass.com
  spf: true
hosts:
- cert_expires: Oct  4 21:57:16 2026 GMT
  host: eonpass.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eon Pass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eon Pass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Eon Pass
provider_slug: eon-pass
slug: eon-pass-domain-security
source_filename: eon-pass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eonpass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:57:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eonpass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eon-pass/refs/heads/main/security/eon-pass-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Anti-Counterfeiting
- Brand Protection
- Artificial Intelligence
- Security
- Investigations
- Enforcement
---
