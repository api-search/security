---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cleverdeck.com
  spf: true
hosts:
- cert_expires: Aug 29 15:50:43 2026 GMT
  host: cleverdeck.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cleverdeck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cleverdeck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cleverdeck
provider_slug: cleverdeck
slug: cleverdeck-domain-security
source_filename: cleverdeck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cleverdeck.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 15:50:43 2026 GMT\n  hsts: false\ndomains:\n- domain: cleverdeck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleverdeck/refs/heads/main/security/cleverdeck-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Education
- Language Learning
- Flashcards
- Spaced Repetition
- EdTech
- iOS
- Mobile App
- Vocabulary
---
