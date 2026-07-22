---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: upcodeacademy.com
  spf: true
hosts:
- cert_expires: Oct  3 00:25:53 2026 GMT
  host: www.upcodeacademy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upcode Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upcode Academy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Upcode Academy
provider_slug: upcode-academy
slug: upcode-academy-domain-security
source_filename: upcode-academy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upcodeacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:25:53 2026 GMT\n  hsts: null\ndomains:\n- domain: upcodeacademy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upcode-academy/refs/heads/main/security/upcode-academy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Education
- Coding Bootcamp
- Training
- Data Science
- Singapore
- Defunct
---
