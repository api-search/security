---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: switchme.in
  spf: false
hosts:
- cert_expires: Sep 19 12:30:42 2026 GMT
  host: switchme.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Switchme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SwitchMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SwitchMe
provider_slug: switchme
slug: switchme-domain-security
source_filename: switchme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: switchme.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 12:30:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: switchme.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/switchme/refs/heads/main/security/switchme-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Fintech
- India
- Lending
- Mobile
- Financial Services
---
