---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thenoor.co
  spf: false
hosts:
- cert_expires: Sep 22 23:30:56 2026 GMT
  host: thenoor.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thenoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheNoor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: TheNoor
provider_slug: thenoor
slug: thenoor-domain-security
source_filename: thenoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thenoor.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:30:56 2026 GMT\n  hsts: false\ndomains:\n- domain: thenoor.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thenoor/refs/heads/main/security/thenoor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Islamic
- Muslim
- Lifestyle App
- Mobile App
- Prayer Times
- Quran
- Consumer App
---
